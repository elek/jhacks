---
creationDate        : 2006-11-16 11:17:59 +0100 
author              : kocka 
title               : maven/maven2/IDE support 
name                : maven/maven2/IDE support 
layout              : wiki 
path                : maven/maven2/IDE support 
date                : 2006-11-16 11:17:59 +0100 
version             : 1 
creator             : kocka 
---
A [maven/maven2](../../maven/maven2.html) eleg frankon tamogatja az [eclipse](../../Eclipse.html) [IDE](../../IDE.html)t, viszont a leszarmaztatott idekkel ([myeclipse](../../myeclipse.html), [websphhere app dev](../../Missing.html)) problemaba utkozhet az ember, amire most egy kis megoldast hozok fel.

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
					<downloadSources>true</downloadSources>
					<wtpversion>1.0</wtpversion>
					<downloadsources>true</downloadsources>
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
