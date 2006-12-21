---
creationDate        : 2006-11-16 11:17:59 +0100 
author              : kocka 
title               : maven/maven2/IDE support 
name                : maven/maven2/IDE support 
layout              : wiki 
path                : maven/maven2/IDE support 
date                : 2006-12-21 09:19:11 +0100 
version             : 7 
creator             : kocka 
---
A [maven/maven2](../../maven/maven2.html) eleg frankon tamogatja az [eclipse](../../Eclipse.html) [IDE](../../IDE.html)t, viszont a leszarmaztatott idekkel ([myeclipse](../../myeclipse.html), [websphere app dev](../../Websphere%20App%20Dev.html)) problemaba utkozhet az ember, amire most egy kis megoldast hozok fel.

Nagyon egyszeru, imadni fogjatok :D

Alaptechnologia: [maven profile](http://maven.apache.org/guides/introduction/introduction-to-profiles.html)

Peldaul egy [webapp](../../webapp.html) eseten az [eclipse](../../Eclipse.html) supportot igy deklaraltad: 

```
			<plugin>
				<groupId>org.apache.maven.plugins</groupId>
				<artifactId>maven-eclipse-plugin</artifactId>
				<version>2.2</version>
				<configuration>
					<workspace>${basedir}</workspace>
					<wtpversion>1.0</wtpversion>
				</configuration>
			</plugin>
```

most jon a zavaro tenyezo hogy nehany szerencses munkatarsnak jutott [myeclipse](../../myeclipse.html) licensz, mas kevesbe szerencsesnek esetleg [websphere app dev](../../Websphere%20App%20Dev.html), es frankon megoldjuk eztet is:

```
	<profiles>

		<profile>
			<activation>
				<property>
					<name>IDE</name>
					<value>myeclipse</value>
				</property>
			</activation>
			<build>
				<plugins>
					<plugin>
						<groupId>org.apache.maven.plugins</groupId>
						<artifactId>maven-eclipse-plugin</artifactId>
						<version>2.2</version>
						<configuration>
							<workspace>${basedir}</workspace>
							<downloadSources>true</downloadSources>
							<additionalBuildcommands>
								<buildcommand>
									com.genuitec.eclipse.j2eedt.core.WebClasspathBuilder
								</buildcommand>
								<buildcommand>
									com.genuitec.eclipse.j2eedt.core.J2EEProjectValidator
								</buildcommand>
								<buildcommand>
									com.genuitec.eclipse.j2eedt.core.DeploymentDescriptorValidator
								</buildcommand>
							</additionalBuildcommands>
							<additionalProjectnatures>
								<projectnature>
									com.genuitec.eclipse.cross.easystruts.eclipse.easystrutsnature
								</projectnature>
								<projectnature>
									com.genuitec.eclipse.j2eedt.core.webnature
								</projectnature>
							</additionalProjectnatures>
							<wtpversion>1.0</wtpversion>
							<downloadsources>true</downloadsources>
						</configuration>
					</plugin>
				</plugins>
			</build>
		</profile>
		<profile>
			<activation>
				<property>
					<name>IDE</name>
					<value>wsad</value>
				</property>
			</activation>
			<build>
				<plugins>
					<plugin>
						<groupId>org.apache.maven.plugins</groupId>
						<artifactId>maven-eclipse-plugin</artifactId>
						<version>2.2</version>
						<configuration>
							<workspace>${basedir}</workspace>
							<downloadSources>true</downloadSources>
							<additionalBuildcommands>
								<buildcommand>
									com.ibm.etools.webtools.LibDirBuilder
								</buildcommand>
								<buildcommand>
									com.ibm.etools.webtools.additions.linksbuilder
								</buildcommand>
								<buildcommand>
									com.ibm.etools.webpage.template.templatebuilder
								</buildcommand>
								<buildcommand>
									com.ibm.etools.siteedit.SiteNavBuilder
								</buildcommand>
								<buildcommand>
									com.ibm.etools.siteedit.SiteUpdateBuilder
								</buildcommand>
								<buildcommand>
									com.ibm.etools.validation.validationbuilder
								</buildcommand>
								<buildcommand>
									com.ibm.etools.webtools.additions.jspcompilationbuilder
								</buildcommand>
								<buildcommand>
									com.ibm.etools.j2ee.LibCopyBuilder
								</buildcommand>
								<buildcommand>
									com.ibm.etools.ctc.serviceprojectbuilder
								</buildcommand>

							</additionalBuildcommands>
							<additionalProjectnatures>
								<projectnature>
									<nature>
										com.ibm.etools.beaninfo.BeaninfoNature
									</nature>
									<nature>
										com.ibm.etools.j2ee.WebNature
									</nature>
									<nature>
										com.ibm.etools.webpage.template.templatenature
									</nature>
									<nature>
										com.ibm.etools.siteedit.WebSiteNature
									</nature>
									<nature>
										com.ibm.etools.ctc.javaprojectnature
									</nature>
									<nature></nature>
								</projectnature>
							</additionalProjectnatures>
							<wtpversion>1.0</wtpversion>
							<downloadsources>true</downloadsources>
						</configuration>
					</plugin>
				</plugins>
			</build>
		</profile>
	</profiles>

```

Innentol aki [myeclipse](../../myeclipse.html)t akar hajtani annak igy kell a [maven](../../maven.html)-nel kigeneraltatni a project descriptorokat:
```
mvn -DIDE=myeclipse eclipse:eclipse
```

Mig a balsorsu [websphere app dev](../../Websphere%20App%20Dev.html) felhasznalok:
```
mvn -DIDE=wsad eclipse:eclipse
```

Ilyen modon fuggetlenne tettuk a projectunket a fejlesztokornyezettol. Azt meg erdemes megjegyezni hogy a leszarmaztatott idek hasznalnak helyenkent nem szabvanyos allomanyokat amiket maguk generalnak, ezeket az eclipse plugin nem tamogatja per pillanat, de lehet oket kezzel editalni.

Szukseg eseten persze a fenti cucchoz hozzaadhatunk [spring](../../spring.html), [struts](../../struts.html) stb project nature-t es buildert.

S lon beke es szeretet a vilagon. Ja ezt az egeszet a [linux 48](../../Linux%2048.html)-ra otlottuk ki, ahol sajna nem tudtuk bevetni a [maven](../../maven.html)t, de azert frankon mukodik.
