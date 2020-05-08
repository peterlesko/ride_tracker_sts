# ride_tracker_sts
chapter_4_completed_up_to_JdbcTemplate_insert_demo, in STS
After Tomca is run I get following output. It appears that server is running, however there is some exception.
Also Hello World! is not printed in browser.

May 08, 2020 8:46:11 PM org.apache.tomcat.util.digester.SetPropertiesRule begin
WARNING: [SetPropertiesRule]{Server/Service/Engine/Host/Context} Setting property 'source' to 'org.eclipse.jst.jee.server:ride_tracker' did not find a matching property.
May 08, 2020 8:46:11 PM org.apache.catalina.startup.VersionLoggerListener log
INFO: Server version:        Apache Tomcat/8.0.36
May 08, 2020 8:46:11 PM org.apache.catalina.startup.VersionLoggerListener log
INFO: Server built:          Jun 9 2016 13:55:50 UTC
May 08, 2020 8:46:11 PM org.apache.catalina.startup.VersionLoggerListener log
INFO: Server number:         8.0.36.0
May 08, 2020 8:46:11 PM org.apache.catalina.startup.VersionLoggerListener log
INFO: OS Name:               Windows 10
May 08, 2020 8:46:11 PM org.apache.catalina.startup.VersionLoggerListener log
INFO: OS Version:            10.0
May 08, 2020 8:46:11 PM org.apache.catalina.startup.VersionLoggerListener log
INFO: Architecture:          amd64
May 08, 2020 8:46:11 PM org.apache.catalina.startup.VersionLoggerListener log
INFO: Java Home:             C:\Program Files\Java\jdk-11.0.3
May 08, 2020 8:46:11 PM org.apache.catalina.startup.VersionLoggerListener log
INFO: JVM Version:           11.0.3+12-LTS
May 08, 2020 8:46:11 PM org.apache.catalina.startup.VersionLoggerListener log
INFO: JVM Vendor:            Oracle Corporation
May 08, 2020 8:46:11 PM org.apache.catalina.startup.VersionLoggerListener log
INFO: CATALINA_BASE:         C:\Users\Pet\Documents\Learning\Pluralsight\Spring\BuildingApplicationsUsingSpringJDBC2\.metadata\.plugins\org.eclipse.wst.server.core\tmp0
May 08, 2020 8:46:11 PM org.apache.catalina.startup.VersionLoggerListener log
INFO: CATALINA_HOME:         C:\dev\tools\apache-tomcat-9.0.34
May 08, 2020 8:46:11 PM org.apache.catalina.startup.VersionLoggerListener log
INFO: Command line argument: -Dcatalina.base=C:\Users\Pet\Documents\Learning\Pluralsight\Spring\BuildingApplicationsUsingSpringJDBC2\.metadata\.plugins\org.eclipse.wst.server.core\tmp0
May 08, 2020 8:46:11 PM org.apache.catalina.startup.VersionLoggerListener log
INFO: Command line argument: -Dcatalina.home=C:\dev\tools\apache-tomcat-9.0.34
May 08, 2020 8:46:11 PM org.apache.catalina.startup.VersionLoggerListener log
INFO: Command line argument: -Dwtp.deploy=C:\Users\Pet\Documents\Learning\Pluralsight\Spring\BuildingApplicationsUsingSpringJDBC2\.metadata\.plugins\org.eclipse.wst.server.core\tmp0\wtpwebapps
May 08, 2020 8:46:11 PM org.apache.catalina.startup.VersionLoggerListener log
INFO: Command line argument: -Dfile.encoding=Cp1252
May 08, 2020 8:46:11 PM org.apache.catalina.core.AprLifecycleListener lifecycleEvent
INFO: The APR based Apache Tomcat Native library which allows optimal performance in production environments was not found on the java.library.path: C:\Program Files\Java\jdk-11.0.3\bin;C:\WINDOWS\Sun\Java\bin;C:\WINDOWS\system32;C:\WINDOWS;C:/Program Files/Java/jdk-11.0.3/bin/server;C:/Program Files/Java/jdk-11.0.3/bin;C:\Program Files (x86)\Intel\iCLS Client\;C:\Program Files\Java\jdk-11.0.3\bin;C:\dev\tools\apache-maven-3.6.1\bin;C:\Program Files (x86)\Common Files\Oracle\Java\javapath;C:\Program Files\Intel\iCLS Client\;C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;C:\Program Files (x86)\NVIDIA Corporation\PhysX\Common;C:\WINDOWS\system32;C:\WINDOWS;C:\WINDOWS\System32\Wbem;C:\WINDOWS\System32\WindowsPowerShell\v1.0\;C:\Program Files\PuTTY\;C:\Program Files\Git\cmd;C:\Program Files\Maven\bin;C:\WINDOWS\System32\OpenSSH\;C:\Program Files (x86)\sbt\bin;C:\Program Files (x86)\scala\bin;C:\Program Files (x86)\Java\jdk1.8.0_171\bin;C:\Program Files\NVIDIA Corporation\NVIDIA NvDLISR;C:\WINDOWS\system32;C:\WINDOWS;C:\WINDOWS\System32\Wbem;C:\WINDOWS\System32\WindowsPowerShell\v1.0\;C:\WINDOWS\System32\OpenSSH\;C:\Program Files\Microsoft\Web Platform Installer\;C:\Users\Pet\AppData\Roaming\nvm;C:\Program Files\nodejs;C:\Program Files\nodejs\;C:\Program Files\Intel\WiFi\bin\;C:\Program Files\Common Files\Intel\WirelessCommon\;C:\Program Files (x86)\Intel\Intel(R) Management Engine Components\DAL;C:\Program Files\Intel\Intel(R) Management Engine Components\DAL;C:\Program Files (x86)\Intel\Intel(R) Management Engine Components\IPT;C:\Program Files\Intel\Intel(R) Management Engine Components\IPT;C:\dev\tools\apache-maven-3.6.1\bin;C:\Users\Pet\Maven\apache-maven-3.2.2\bin;C:\Gradle\gradle-6.1\bin;C:\Gradle\gradle-6.1\bin;C:\Program Files\Java\jdk-11.0.3\bin;C:\Program Files\PostgreSQL\12\bin;C:\Program Files\Notepad++;C:\Users\Pet\AppData\Local\Microsoft\WindowsApps;C:\Users\Pet\AppData\Local\Programs\Microsoft VS Code\bin;C:\Users\Pet\AppData\Roaming\nvm;C:\Program Files\nodejs;C:\Users\Pet\AppData\Roaming\npm;C:\Users\Pet\AppData\Local\GitHubDesktop\bin;C:\Users\Pet\AppData\Local\atom\bin;C:\Users\Pet\AppData\Local\Microsoft\WindowsApps;C:\dev\tools\sts-4.6.1.RELEASE;;.
May 08, 2020 8:46:11 PM org.apache.catalina.core.JreMemoryLeakPreventionListener lifecycleEvent
SEVERE: Failed to trigger creation of the GC Daemon thread during Tomcat start to prevent possible memory leaks. This is expected on non-Sun JVMs.
java.lang.ClassNotFoundException: sun.misc.GC
	at java.base/java.net.URLClassLoader.findClass(URLClassLoader.java:471)
	at java.base/java.lang.ClassLoader.loadClass(ClassLoader.java:588)
	at java.base/java.lang.ClassLoader.loadClass(ClassLoader.java:521)
	at java.base/java.lang.Class.forName0(Native Method)
	at java.base/java.lang.Class.forName(Class.java:315)
	at org.apache.catalina.core.JreMemoryLeakPreventionListener.lifecycleEvent(JreMemoryLeakPreventionListener.java:286)
	at org.apache.catalina.util.LifecycleSupport.fireLifecycleEvent(LifecycleSupport.java:95)
	at org.apache.catalina.util.LifecycleBase.fireLifecycleEvent(LifecycleBase.java:90)
	at org.apache.catalina.util.LifecycleBase.setStateInternal(LifecycleBase.java:394)
	at org.apache.catalina.util.LifecycleBase.init(LifecycleBase.java:99)
	at org.apache.catalina.startup.Catalina.load(Catalina.java:580)
	at org.apache.catalina.startup.Catalina.load(Catalina.java:603)
	at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at java.base/jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.base/java.lang.reflect.Method.invoke(Method.java:566)
	at org.apache.catalina.startup.Bootstrap.load(Bootstrap.java:310)
	at org.apache.catalina.startup.Bootstrap.main(Bootstrap.java:484)

May 08, 2020 8:46:11 PM org.apache.coyote.AbstractProtocol init
INFO: Initializing ProtocolHandler ["http-nio-8080"]
May 08, 2020 8:46:11 PM org.apache.tomcat.util.net.NioSelectorPool getSharedSelector
INFO: Using a shared selector for servlet write/read
May 08, 2020 8:46:11 PM org.apache.coyote.AbstractProtocol init
INFO: Initializing ProtocolHandler ["ajp-nio-8009"]
May 08, 2020 8:46:11 PM org.apache.tomcat.util.net.NioSelectorPool getSharedSelector
INFO: Using a shared selector for servlet write/read
May 08, 2020 8:46:11 PM org.apache.catalina.startup.Catalina load
INFO: Initialization processed in 861 ms
May 08, 2020 8:46:11 PM org.apache.catalina.core.StandardService startInternal
INFO: Starting service Catalina
May 08, 2020 8:46:11 PM org.apache.catalina.core.StandardEngine startInternal
INFO: Starting Servlet Engine: Apache Tomcat/8.0.36
May 08, 2020 8:46:11 PM org.apache.catalina.loader.WebappLoader buildClassPath
INFO: Unknown loader jdk.internal.loader.ClassLoaders$AppClassLoader@6e5e91e4 class jdk.internal.loader.ClassLoaders$AppClassLoader
May 08, 2020 8:46:12 PM org.apache.jasper.servlet.TldScanner scanJars
INFO: At least one JAR was scanned for TLDs yet contained no TLDs. Enable debug logging for this logger for a complete list of JARs that were scanned but no TLDs were found in them. Skipping unneeded JARs during scanning can improve startup time and JSP compilation time.
May 08, 2020 8:46:12 PM org.apache.catalina.util.SessionIdGeneratorBase createSecureRandom
INFO: Creation of SecureRandom instance for session ID generation using [SHA1PRNG] took [144] milliseconds.
May 08, 2020 8:46:12 PM org.apache.catalina.loader.WebappLoader buildClassPath
INFO: Unknown loader jdk.internal.loader.ClassLoaders$AppClassLoader@6e5e91e4 class jdk.internal.loader.ClassLoaders$AppClassLoader
May 08, 2020 8:46:13 PM org.apache.jasper.servlet.TldScanner scanJars
INFO: At least one JAR was scanned for TLDs yet contained no TLDs. Enable debug logging for this logger for a complete list of JARs that were scanned but no TLDs were found in them. Skipping unneeded JARs during scanning can improve startup time and JSP compilation time.
May 08, 2020 8:46:13 PM org.apache.catalina.core.ApplicationContext log
INFO: No Spring WebApplicationInitializer types detected on classpath
May 08, 2020 8:46:13 PM org.apache.coyote.AbstractProtocol start
INFO: Starting ProtocolHandler ["http-nio-8080"]
May 08, 2020 8:46:13 PM org.apache.coyote.AbstractProtocol start
INFO: Starting ProtocolHandler ["ajp-nio-8009"]
May 08, 2020 8:46:13 PM org.apache.catalina.startup.Catalina start
INFO: Server startup in 2349 ms


After excuting testCreateRide() Im getting following output and exception.

May 08, 2020 8:49:53 PM org.apache.catalina.core.ApplicationContext log
INFO: Initializing Spring FrameworkServlet 'rideTrackerServlet'
2020-05-08 20:49:53 INFO  DispatcherServlet:489 - FrameworkServlet 'rideTrackerServlet': initialization started
2020-05-08 20:49:53 INFO  XmlWebApplicationContext:582 - Refreshing WebApplicationContext for namespace 'rideTrackerServlet-servlet': startup date [Fri May 08 20:49:53 BST 2020]; root of context hierarchy
2020-05-08 20:49:53 INFO  XmlBeanDefinitionReader:317 - Loading XML bean definitions from ServletContext resource [/WEB-INF/config/servlet-config.xml]
2020-05-08 20:49:53 INFO  XmlBeanDefinitionReader:317 - Loading XML bean definitions from class path resource [jdbc-config.xml]
2020-05-08 20:49:54 INFO  RequestMappingHandlerMapping:543 - Mapped "{[/ride],methods=[PUT]}" onto public com.pluralsight.model.Ride com.pluralsight.controller.RideController.createRide(com.pluralsight.model.Ride)
2020-05-08 20:49:54 INFO  RequestMappingHandlerMapping:543 - Mapped "{[/rides],methods=[GET]}" onto public java.util.List<com.pluralsight.model.Ride> com.pluralsight.controller.RideController.getRides()
2020-05-08 20:49:55 INFO  RequestMappingHandlerAdapter:534 - Looking for @ControllerAdvice: WebApplicationContext for namespace 'rideTrackerServlet-servlet': startup date [Fri May 08 20:49:53 BST 2020]; root of context hierarchy
2020-05-08 20:49:55 INFO  RequestMappingHandlerAdapter:534 - Looking for @ControllerAdvice: WebApplicationContext for namespace 'rideTrackerServlet-servlet': startup date [Fri May 08 20:49:53 BST 2020]; root of context hierarchy
2020-05-08 20:49:55 INFO  DriverManagerDataSource:133 - Loaded JDBC driver: com.mysql.cj.jdbc.Driver
2020-05-08 20:49:55 INFO  DispatcherServlet:508 - FrameworkServlet 'rideTrackerServlet': initialization completed in 2201 ms
May 08, 2020 8:49:55 PM org.apache.catalina.core.StandardWrapperValve invoke
SEVERE: Servlet.service() for servlet [rideTrackerServlet] in context with path [/ride_tracker] threw exception [Request processing failed; nested exception is org.springframework.jdbc.CannotGetJdbcConnectionException: Could not get JDBC Connection; nested exception is java.sql.SQLException: No suitable driver found for jdbc:msql://localhost:3306/ride_tracker] with root cause
java.sql.SQLException: No suitable driver found for jdbc:msql://localhost:3306/ride_tracker
	at java.sql/java.sql.DriverManager.getConnection(DriverManager.java:702)
	at java.sql/java.sql.DriverManager.getConnection(DriverManager.java:189)
	at org.springframework.jdbc.datasource.DriverManagerDataSource.getConnectionFromDriverManager(DriverManagerDataSource.java:153)
	at org.springframework.jdbc.datasource.DriverManagerDataSource.getConnectionFromDriver(DriverManagerDataSource.java:144)
	at org.springframework.jdbc.datasource.AbstractDriverBasedDataSource.getConnectionFromDriver(AbstractDriverBasedDataSource.java:196)
	at org.springframework.jdbc.datasource.AbstractDriverBasedDataSource.getConnection(AbstractDriverBasedDataSource.java:159)
	at org.springframework.jdbc.datasource.DataSourceUtils.doGetConnection(DataSourceUtils.java:111)
	at org.springframework.jdbc.datasource.DataSourceUtils.getConnection(DataSourceUtils.java:77)
	at org.springframework.jdbc.core.JdbcTemplate.execute(JdbcTemplate.java:619)
	at org.springframework.jdbc.core.JdbcTemplate.update(JdbcTemplate.java:870)
	at org.springframework.jdbc.core.JdbcTemplate.update(JdbcTemplate.java:931)
	at org.springframework.jdbc.core.JdbcTemplate.update(JdbcTemplate.java:941)
	at com.pluralsight.repository.RideRepositoryImpl.createRide(RideRepositoryImpl.java:19)
	at com.pluralsight.service.RideServiceImpl.createRide(RideServiceImpl.java:19)
	at com.pluralsight.controller.RideController.createRide(RideController.java:22)
	at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at java.base/jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.base/java.lang.reflect.Method.invoke(Method.java:566)
	at org.springframework.web.method.support.InvocableHandlerMethod.doInvoke(InvocableHandlerMethod.java:205)
	at org.springframework.web.method.support.InvocableHandlerMethod.invokeForRequest(InvocableHandlerMethod.java:133)
	at org.springframework.web.servlet.mvc.method.annotation.ServletInvocableHandlerMethod.invokeAndHandle(ServletInvocableHandlerMethod.java:116)
	at org.springframework.web.servlet.mvc.method.annotation.RequestMappingHandlerAdapter.invokeHandlerMethod(RequestMappingHandlerAdapter.java:827)
	at org.springframework.web.servlet.mvc.method.annotation.RequestMappingHandlerAdapter.handleInternal(RequestMappingHandlerAdapter.java:738)
	at org.springframework.web.servlet.mvc.method.AbstractHandlerMethodAdapter.handle(AbstractHandlerMethodAdapter.java:85)
	at org.springframework.web.servlet.DispatcherServlet.doDispatch(DispatcherServlet.java:963)
	at org.springframework.web.servlet.DispatcherServlet.doService(DispatcherServlet.java:897)
	at org.springframework.web.servlet.FrameworkServlet.processRequest(FrameworkServlet.java:970)
	at org.springframework.web.servlet.FrameworkServlet.doPut(FrameworkServlet.java:883)
	at javax.servlet.http.HttpServlet.service(HttpServlet.java:651)
	at org.springframework.web.servlet.FrameworkServlet.service(FrameworkServlet.java:846)
	at javax.servlet.http.HttpServlet.service(HttpServlet.java:729)
	at org.apache.catalina.core.ApplicationFilterChain.internalDoFilter(ApplicationFilterChain.java:292)
	at org.apache.catalina.core.ApplicationFilterChain.doFilter(ApplicationFilterChain.java:207)
	at org.apache.tomcat.websocket.server.WsFilter.doFilter(WsFilter.java:52)
	at org.apache.catalina.core.ApplicationFilterChain.internalDoFilter(ApplicationFilterChain.java:240)
	at org.apache.catalina.core.ApplicationFilterChain.doFilter(ApplicationFilterChain.java:207)
	at org.apache.catalina.core.StandardWrapperValve.invoke(StandardWrapperValve.java:212)
	at org.apache.catalina.core.StandardContextValve.invoke(StandardContextValve.java:106)
	at org.apache.catalina.authenticator.AuthenticatorBase.invoke(AuthenticatorBase.java:502)
	at org.apache.catalina.core.StandardHostValve.invoke(StandardHostValve.java:141)
	at org.apache.catalina.valves.ErrorReportValve.invoke(ErrorReportValve.java:79)
	at org.apache.catalina.valves.AbstractAccessLogValve.invoke(AbstractAccessLogValve.java:616)
	at org.apache.catalina.core.StandardEngineValve.invoke(StandardEngineValve.java:88)
	at org.apache.catalina.connector.CoyoteAdapter.service(CoyoteAdapter.java:528)
	at org.apache.coyote.http11.AbstractHttp11Processor.process(AbstractHttp11Processor.java:1099)
	at org.apache.coyote.AbstractProtocol$AbstractConnectionHandler.process(AbstractProtocol.java:670)
	at org.apache.tomcat.util.net.NioEndpoint$SocketProcessor.doRun(NioEndpoint.java:1520)
	at org.apache.tomcat.util.net.NioEndpoint$SocketProcessor.run(NioEndpoint.java:1476)
	at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1128)
	at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:628)
	at org.apache.tomcat.util.threads.TaskThread$WrappingRunnable.run(TaskThread.java:61)
	at java.base/java.lang.Thread.run(Thread.java:834)



