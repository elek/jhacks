---
creationDate        : 2008-11-02 20:16:01 +0100 
author              : zmb 
title               : WTF/Parameterezes 
name                : WTF/Parameterezes 
layout              : wiki 
path                : WTF/Parameterezes 
date                : 2008-11-02 20:16:01 +0100 
version             : 1 
creator             : zmb 
---
Elso pelda egy php fejleszto munkajat dicseri. Nyilvan hallott arrol, hogy a sok parameter egy fuggvenyben rossz dolog, ezert az osszes parametert egy stringbe gyomoszoli bele, amit a fuggvenyen belul szetrobbant, es azokkal dolgozik tovabb:

```
function fn($args = '') {
	$args = parse_args($args);

	isset($args['order']) ? $order=$args['order'] : $order = 'time';
	isset($args['sort']) ? $sort=$args['sort'] : $sort = 'DESC';
	isset($args['thecat']) ? $thecat=$args['thecat'] : $thecat = 'all';
	...
}
```

A kovetkezo ket kod (immaron javaban) alkotoja viszont nem hallott arrol, hogy a tul sok parameter nem feltetlen szerencses (kulon felhivnam a fuggveny roppant frappans nevere).

```
public Vector<OrderEntry2> getOrders2(String user, String[] accountGroups, String supplier, String date, String date2, int hour, int hour2, String udate, String udate2, String deliv, String orderId, int closingType, String payMode, String remark, String billName, String delivName, String sdate, String sdate2, String status, String limit, Integer top100, int hpayedFilter, boolean allItemsOnStock, boolean onlyAdminOrders, String closingts) {
```

Termeszetesen a parameterek egy resze opcionalis, ami - ugyancsak termeszetesen - sehol nincsen leirva. Ha kivancsi vagy ra, akkor csak vegig kell bogaraszni a par oldalnyi kodot (ami egy sql-t kolbaszol ossze).

A kovetkezo kis kodocska egy alaposan atgondolt konstruktort mutat be:

```
public OrderHead(int orderId, String userId, boolean isRetail, Integer courierId, OrderType orderType, String transid,
			String currency, double currencyRate, int payMethod, String delivery, double deliveryCost, double deliveryDisc, boolean billRequired, String billName,
			Integer billCountryId, String billZip, String billCity, String billStreet, String billVatNumber, String name, int countryId, String zip, String building, String city,
			String street, String phone, String cellular, String email,String courierRemark, String remarks, double finaltotal, Date orderDate, Date undertakenDate, boolean isfaked, String domain,boolean allItemsOnStock,
			List<OrderDevalueInformation> odInfo, boolean adminOrder,String adminRemark, Integer affiliateId) {
```

Megfigyelheto, hogy mindenfele cim adatokat is megkap parameterben. Gyakorlatilag az egy objektum, de ahelyett, hogy a komplett objektumot adna at, inkabb minden mezot kulon (biztos azert, hogy csokkenjen a fuggoseg).
