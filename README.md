# AppPortfolio

Test connector usage:

1. Check out the test connector JavaSDK package in your local workspace
2. Specify a connector id in the setup.properties file correspond to Agents table in use 
3. Specify a SMS endpoint (e.g. https://0.0.0.0:8001) in the setup.properties file for test connector to send responses to
4. Specify any mocking data you want to each task connector to provide in testdata.yml
5. Compile & run the TestConnector program (e.g. java com.amazonaws.servermigration.test.TestConnector)
6. Start testing your workflows by initiating connector tasks from SMS client calls

Note: Before running the test connector, you will need to add the compiled classes to the current classpath by doing below:

export CLASSPATH=`brazil-path build.classpath`;                

export CLASSPATH=$CLASSPATH:./build/lib/AWSServerMigrationSDKJavaClient-1.0.jar;

For more information:
Test connector wiki: https://w.amazon.com/bin/view/ServerMigrationService/TestConnector/
Contact: zxq@amazon.com

