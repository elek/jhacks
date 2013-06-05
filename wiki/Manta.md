---
creationDate: 1129810599777 
author: kocka 
contentAuthor: kocka 
title: Manta 
contentUpdateDate: 1129899123467 
name: Manta 
layout: wiki 
date: 1129899123467 
creator: kocka 
---
http://www.mantamq.org/

Egy Dual kereskedelmi/[GPL](GPL.html) licenszelesu (szoval nem valami baratsagos) [JMS](JMS.html) rendszer. Az sajatos erdekessege az hogy multicast-tal lehet neki uzengetni, es ha valamelyik szerver kihal a clusterbol, akkor meg mindig megy az egesz.

Egyebkent a forraskodja rendkivul [gyanus](gyanus.html):
{% highlight java %}

    private MantaAgent() \{
        try \{

            mantaHome = System.getProperty(MantaAgentConstants.MANTA_HOME);
            if (mantaHome == null) \{
                System.out.println("Manta home was not set! - Please set the system property 'mantaHome' to your manta home folder in the system property.");
                System.out
                        .println("In order for manta to work properly this property needs to be set to the folder were the manta folders exist (config, persistent, logs and more)");
                mantaHome = ".";
            \}
            System.out.println("property 'mantaHome'=" + mantaHome);

            //validate that the params exist end notify about it
            configurationFolder = mantaHome + "/config/";
            defaultConfigurationFile = configurationFolder + "/default_config.params";
            agentConfigurationFile = configurationFolder + "/component_config.params";
            worldXmlFilePath = configurationFolder + "/world.xml";
            pesistentFolder = mantaHome + "/persistent/";
            

            System.out.println("property 'configurationFolder'=" + configurationFolder);
            FileOrFolderExists(configurationFolder);
            System.out.println("property 'defaultConfigurationFile'=" + defaultConfigurationFile);
            FileOrFolderExists(defaultConfigurationFile);
            System.out.println("property 'agentConfigurationFile'=" + agentConfigurationFile);
            FileOrFolderExists(agentConfigurationFile);
            System.out.println("property 'worldXmlFilePath'=" + worldXmlFilePath);
            FileOrFolderExists(worldXmlFilePath);
            System.out.println("property 'pesistentFolder'=" + pesistentFolder);
            FileOrFolderExists(pesistentFolder);
            
            PersistentConst.setPersistantDir(pesistentFolder)  ;
            

        \}
        catch (Throwable t) \{
            t.printStackTrace();
        \}//catch

    \}//MantaAgent

{% endhighlight %}
