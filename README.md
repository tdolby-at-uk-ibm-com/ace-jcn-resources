# ace-jcn-resources
Simple application showing loading of Java resources

```
tdolby:/$ mqsicreateworkdir ~/tmp/jcn-resources-work-dir
mqsicreateworkdir: Copying sample server.config.yaml to work directory
1 file(s) copied.
Successful command completion.

tdolby:/$ mqsibar -c -w ~/tmp/jcn-resources-work-dir -a ~/git/ace-jcn-resources/TimerJCNApplication/TimerJCNApplication.bar 
Generating runtime objects: '/home/tdolby/tmp/jcn-resources-work-dir/run' ...

BIP8071I: Successful command completion.

tdolby:/$ IntegrationServer -w ~/tmp/jcn-resources-work-dir
2022-06-01 02:59:24.357430: BIP1990I: Integration server 'jcn-resources-work-dir' starting initialization; version '12.0.4.0' (64-bit) 
2022-06-01 02:59:24.362494: BIP9905I: Initializing resource managers. 
2022-06-01 02:59:28.294536: BIP9906I: Reading deployed resources. 
2022-06-01 02:59:28.297792: BIP9907I: Initializing deployed resources. 
2022-06-01 02:59:28.299858: BIP2155I: About to 'Initialize' the deployed resource 'TimerJCNApplication' of type 'Application'. 
2022-06-01 02:59:28.503694: BIP2155I: About to 'Start' the deployed resource 'TimerJCNApplication' of type 'Application'. 
2022-06-01 02:59:28.504052: BIP2269I: Deployed resource 'ResourceTestFlow' (uuid='ResourceTestFlow',type='MessageFlow') started successfully. 
2022-06-01 02:59:28.507520: BIP3051E: Error message '( ['json' : 0x7f32d0037290]
  (0x01000000:Object):Data = (
    (0x03000000:NameValue):testValue = 'TestDataFromFile' (CHARACTER)
  )
)
' from trace node 'ResourceTestFlow.Trace'. 
2022-06-01 02:59:29.050880: BIP2866I: IBM App Connect Enterprise administration security is inactive. 
2022-06-01 02:59:29.065576: BIP3132I: The HTTP Listener has started listening on port '7600' for 'RestAdmin http' connections. 
2022-06-01 02:59:29.074100: BIP1991I: Integration server has finished initialization. 
```
