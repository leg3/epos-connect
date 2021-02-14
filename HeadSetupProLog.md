Info:IUILog

```bash
Info:IUILog : SoftPhoneInfo											                                # Returns a simple soft phone name without version information
Info:IUILog : DeviceInfo											                                # Returns device name and its current configuration options at that timestamp in the log
``` 

Info:AgentApp

```bash
Info:AgentApp::getTenantInfo											                            # Returns the configuration values of the current tennant
Info:AgentApp::getDetails											                                # Returns detailed agent debug info in anonymized format
Info:AgentApp::handleCCEvents
```

Info:RestClient

```bash
Info:RestClient::post
Info:RestClient::post : Request:POST / HTTP/1.1									                    # Precedes a JSON payload header
```
 
Info:CCallControlAdapter

```bash
Info:CCallControlAdapter::updateSoftphoneStatus
Info:CCallControlAdapter::getDeviceConfig
Info:CCallControlAdapter::UpdateSoftphoneList : Available list of softphone from CC engine:			# Returns a JSON payload of the name, vendor, and version of softphones
```

Info:CCSoftPhoneStatusPriority

```bash
Info:CCSoftPhoneStatusPriority::saveSoftphoneStatus								                    # Returns the name and state of the softphone
Info:CCSoftPhoneStatusPriority::setSoftPhoneStatus								                    # The event that sets the value
```
 
Info:CManagePostRequest::

```bash
Info:CManagePostRequest::ManageAgentRegistration :								                    # Returns the agent API URL endpoint - https://api.enterprise.eposaudio.com/api/agent
Info:CManagePostRequest::ManageHeartBeat :									                        # Returns the heartbeat API URL endpoint - https://api.enterprise.eposaudio.com/api/ManageAgent/Heartbeat/
Info:CManagePostRequest::ManageGetADQuery :									                        # Returns the ADQuery API URL endpoint - https://api.enterprise.eposaudio.com/api/ManageAgent/GetAdQuery/
Info:CManagePostRequest::ManageGetUpdates : 									                    # Returns the software and firmware update API URL endpoint https://api.enterprise.eposaudio.com/api/ManageAgent/GetUpdates


Info:CManagePostRequest::PostReqDownloadStatus : 								                    # https://api.enterprise.eposaudio.com/api/ManageAgent/DownloadAcknowledgement/
Info:CManagePostRequest::ManageCCConfig : 									                        # https://api.enterprise.eposaudio.com/api/ManageAgent/UpdateCCConfig/
Info:CManagePostRequest::ManageGetAllUpdates : 									                    # https://api.enterprise.eposaudio.com/api/ManageAgent/GetAllUpdatesAndConfigs
Info:CManagePostRequest::ManageSoftPhoneDetails : 								                    # https://api.enterprise.eposaudio.com/api/ManageAgent/UpdateSoftPhone
Info:CManagePostRequest::ManageSoftPhoneDetails : 								                    # https://api.enterprise.eposaudio.com/api/ManageAgent/UpdateSoftPhoneLog
Info:CManagePostRequest::ManageDevicePluginData : 								                    # https://api.enterprise.eposaudio.com/api/ManageAgent/DeviceConnect
Info:CManagePostRequest::ManageDeviceUnPluginData : 								                # https://api.enterprise.eposaudio.com/api/ManageAgent/DeviceDisconnect
Info:CManagePostRequest::DeviceUpdateStatus : 									                    # https://api.enterprise.eposaudio.com/api/ManageAgent/UpdatesAcknowledgement/

Info:CManagePostRequest::ManageAgentRegistration : Rest->Response For Agent Registration Request:
```

Command strings

```bash
{"Command":												                                            # Find each command string

{"Command":"APP_DVC_CON_REQ"										                                # Device connection request
{"Command":"APP_DVC_DSCON_REQ"										                                # Device disconnection request
{"Command":"APP_SOFTPHONE_UPDATE_REQ"									                            # Softphone(s) Name and version update displayed that timestamp
{"Command":"APP_CC_CONFIG_UPDATE_REQ"									                            # Call control config update at displayed timestamp
{"Command":"APP_DVC_SYNC_REQ"
{"Command":"APP_GET_ALL_UPDT_REQ"

{"Command":"SRV_HB_ACK"
{"Command":"SRV_DVC_CON_ACK"
{"Command":"SRV_DVC_DSCON_ACK"
{"Command":"SRV_DVC_SYNC_ACK"
{"Command":"SRV_CC_CONFIG_UPDATE_SUCCESS_ACK"
{"Command":"SRV_CALLDURATION_UPDATE_SUCCESS_ACK"
{"Command":"SRV_SOFTPHONE_UPDATE_SUCCESS_ACK"

{"AgentDetails":											                                        # EPOS Connect Version and tenant information
{"CallDurationDetails":
{"EventType":
{"FeatureName":
```