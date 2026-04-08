# Qilin Ransomware EDR/AV Killer - Targeted Drivers & Executables

> **Source**: Reverse-engineered from the Qilin EDR killer PE binary  
> **Reference**: [Talos Intelligence - Qilin EDR Killer](https://blog.talosintelligence.com/qilin-edr-killer/)  


---

## Table of Contents

- [Targeted Executables (Processes)](#targeted-executables-processes)
- [Targeted Kernel Drivers](#targeted-kernel-drivers)
- [Vulnerable Drivers Used by the Killer](#vulnerable-drivers-used-by-the-killer)

---

## Targeted Executables (Processes)

### Microsoft Defender / Windows Security

| # | Process Name |
|---|-------------|
| 1 | MpCmdRun.exe |
| 2 | MsMpEng.exe |
| 3 | MsMpEngCP.exe |
| 4 | MsSense.exe |
| 5 | SecurityHealthService.exe |
| 6 | uhssvc.exe |

### Kaspersky

| # | Process Name |
|---|-------------|
| 1 | avp.exe |
| 2 | klnagent.exe |
| 3 | avpsus.exe |
| 4 | avpui.exe |
| 5 | kavfs.exe |
| 6 | kavfsgt.exe |
| 7 | kavfswh.exe |
| 8 | kavfswp.exe |
| 9 | kavtray.exe |
| 10 | ebloader.exe |
| 11 | klcsldcl.exe |
| 12 | soyuz.exe |
| 13 | proton.exe |
| 14 | vapm.exe |

### Sophos

| # | Process Name |
|---|-------------|
| 1 | SEDService.exe |
| 2 | hmpalert.exe |
| 3 | SSPService.exe |
| 4 | SophosNtpService.exe |
| 5 | SophosNetFilter.exe |
| 6 | McsAgent.exe |
| 7 | McsClient.exe |
| 8 | SophosFS.exe |
| 9 | SophosFileScanner.exe |
| 10 | SophosHealth.exe |
| 11 | Sophos.Encryption.BitLockerService.exe |
| 12 | SophosLiveQueryService.exe |
| 13 | SophosOsquery.exe |
| 14 | Sophos UI.exe |
| 15 | SophosFIMService.exe |

### ESET

| # | Process Name |
|---|-------------|
| 1 | ERAAgent.exe |
| 2 | efwd.exe |
| 3 | egui.exe |
| 4 | eguiProxy.exe |
| 5 | ekrn.exe |
| 6 | eOppFrame.exe |
| 7 | EIConnector.exe |
| 8 | EIConnectorProxy.exe |

### SentinelOne

| # | Process Name |
|---|-------------|
| 1 | SentinelAgent.exe |
| 2 | SentinelServiceHost.exe |
| 3 | SentinelStaticEngine.exe |
| 4 | SentinelStaticEngineScanner.exe |
| 5 | SentinelUI.exe |
| 6 | SentinelHelperService.exe |
| 7 | SentinelAgentWorker.exe |
| 8 | SentinelMemoryScanner.exe |

### CrowdStrike Falcon

| # | Process Name |
|---|-------------|
| 1 | CSFalconContainer.exe |
| 2 | CSFalconService.exe |
| 3 | CSCOMUtils.exe |
| 4 | CSDeviceControlSupportTool.exe |
| 5 | CSFalconController.exe |
| 6 | CSFirmwareAnalysisSupportTool.exe |
| 7 | CsScan.exe |
| 8 | CsScanCli.exe |
| 9 | CSSensorSettings.exe |

### Trend Micro

| # | Process Name |
|---|-------------|
| 1 | pccntupd.exe |
| 2 | xpupg.exe |
| 3 | svcGenericHost.exe |
| 4 | HostedAgent.exe |
| 5 | logWriter.exe |
| 6 | TMCPMCLI.exe |
| 7 | HostedTelemetry.exe |
| 8 | TMCPMAdapter.exe |
| 9 | TmListen.exe |
| 10 | PccNtMon.exe |
| 11 | TmSSClient.exe |
| 12 | TmCCSF.exe |
| 13 | TmsaInstance64.exe |
| 14 | Ntrtscan.exe |
| 15 | TmWSCSvc.exe |
| 16 | TMBMSRV.exe |
| 17 | DbServer.exe |
| 18 | ofcDdaSvr.exe |
| 19 | OfcLogReceiverSvc.exe |
| 20 | OfcService.exe |
| 21 | OSCEIntegrationService.exe |
| 22 | AU_FRS.exe |
| 23 | CpuCtrl.exe |
| 24 | iCRCService.exe |

### McAfee / Trellix

| # | Process Name |
|---|-------------|
| 1 | masvc.exe |
| 2 | macompatsvc.exe |
| 3 | mfemactl.exe |
| 4 | macmnsvc.exe |
| 5 | mfemms.exe |
| 6 | mcshield.exe |
| 7 | mfeesp.exe |
| 8 | mfefw.exe |
| 9 | mfehcs.exe |
| 10 | mfeatp.exe |
| 11 | mfeensppl.exe |
| 12 | mfetp.exe |
| 13 | mfevtps.exe |
| 14 | mfewc.exe |
| 15 | mfewch.exe |
| 16 | UpdaterUI.exe |
| 17 | mctray.exe |
| 18 | MFEConsole.exe |

### FireEye / Trellix XDR

| # | Process Name |
|---|-------------|
| 1 | xagt.exe |
| 2 | xagtnotif.exe |
| 3 | xagtui.exe |

### Symantec / Broadcom (Symantec Endpoint Protection)

| # | Process Name |
|---|-------------|
| 1 | httpd.exe |
| 2 | rotatelogs.exe |
| 3 | SemLaunchSvc.exe |
| 4 | SemSvc.exe |
| 5 | ccSvcHst.exe |
| 6 | sepWscSvc64.exe |
| 7 | webextbridge.exe |
| 8 | SmcGui.exe |
| 9 | SymCorpUI.exe |

### Bitdefender

| # | Process Name |
|---|-------------|
| 1 | bdredline.exe |
| 2 | EPConsole.exe |
| 3 | EPHost.Integrity.exe |
| 4 | EPIntegrationService.exe |
| 5 | EPProtectedService.exe |
| 6 | EPSecurityService.exe |
| 7 | EPUpdateService.exe |
| 8 | ARWSRVC.EXE |
| 9 | BDSSVC.EXE |
| 10 | accasrvc.exe |
| 11 | REPRSVC.EXE |
| 12 | QUHLPSVC.EXE |
| 13 | spsvc.exe |
| 14 | SCANWSCS.EXE |
| 15 | emlproxy.exe |
| 16 | SAPISSVC.EXE |
| 17 | SCANNER.EXE |
| 18 | scsecsvc.exe |
| 19 | bssiss.exe |
| 20 | umngrsvc.exe |
| 21 | acassrvc.exe |

### Webroot

| # | Process Name |
|---|-------------|
| 1 | WRSkyClient.x64.exe |
| 2 | WRCoreService.x64.exe |
| 3 | WRSkyCommandsClient.exe |
| 4 | WREDRS.x64.exe |
| 5 | WRSA.exe |

### Panda Security (WatchGuard)

| # | Process Name |
|---|-------------|
| 1 | AgentSvc.exe |
| 2 | PSANHost.exe |
| 3 | pselamsvc.exe |
| 4 | PSUAMain.exe |
| 5 | PSUAService.exe |
| 6 | PSNWSC.exe |

### Sangfor EDR

| # | Process Name |
|---|-------------|
| 1 | edr_monitor.exe |
| 2 | edr_agent.exe |
| 3 | sfavsvc.exe |
| 4 | sfupdatemgr.exe |
| 5 | xs_agent.exe |
| 6 | ipc_proxy.exe |
| 7 | abs_deployer.exe |
| 8 | sfavroguedf.exe |
| 9 | eaio_service.exe |
| 10 | eaio_agent.exe |
| 11 | sfavbdup.exe |
| 12 | sfpatch.exe |
| 13 | sfavtray.exe |
| 14 | sfavui.exe |

### Fortinet FortiEDR

| # | Process Name |
|---|-------------|
| 1 | ASCService.exe |
| 2 | AutoUpdate.exe |
| 3 | FortiEDRCollectorService.exe |
| 4 | FortiEDRAvScanner.exe |
| 5 | FortiEDRCollector.exe |

### Avast

| # | Process Name |
|---|-------------|
| 1 | aswEngSrv.exe |
| 2 | aswidsagent.exe |
| 3 | aswToolsSvc.exe |
| 4 | AvastSvc.exe |
| 5 | AvastUI.exe |
| 6 | bcc.exe |
| 7 | bccavsvc.exe |

### Cylance (BlackBerry)

| # | Process Name |
|---|-------------|
| 1 | CylanceSvc.exe |
| 2 | CylanceUI.exe |
| 3 | CyUpdate.exe |

### Qihoo 360

| # | Process Name |
|---|-------------|
| 1 | helper_64.exe |
| 2 | HipsDaemon.exe |
| 3 | HipsTray.exe |
| 4 | usysdiag.exe |
| 5 | wsctrlsvc.exe |
| 6 | ZhuDongFangYu.exe |
| 7 | 360epp.exe |
| 8 | eppcontainer.exe |
| 9 | eppservice.exe |
| 10 | udisktoolui.exe |
| 11 | 360qbus.exe |
| 12 | 360Tray.exe |
| 13 | 360sd.exe |
| 14 | 360safe.exe |
| 15 | 360rp.exe |
| 16 | 360leakfixer.exe |

### QAX (Qi-Anxin)

| # | Process Name |
|---|-------------|
| 1 | QAXrps.exe |
| 2 | LogService.exe |
| 3 | QAXDownMgr.exe |
| 4 | QAXEntClient.exe |
| 5 | QAXSafe.exe |
| 6 | QAXTray.exe |

### F-Secure / WithSecure

| # | Process Name |
|---|-------------|
| 1 | bwserver.exe |
| 2 | fsdevcon.exe |
| 3 | fshoster32.exe |
| 4 | fs_ui_32.exe |
| 5 | fshoster64.exe |
| 6 | wsmain.exe |
| 7 | FsPisces.exe |
| 8 | fsulprothoster.exe |
| 9 | ICM-Service-NET.exe |
| 10 | UM_Interface.exe |

### Check Point / ZoneAlarm

| # | Process Name |
|---|-------------|
| 1 | zatray.exe |
| 2 | vsmon.exe |
| 3 | cscm.exe |
| 4 | iptray.exe |
| 5 | sfc.exe |

### ThreatLocker

| # | Process Name |
|---|-------------|
| 1 | threatlockerservice.exe |
| 2 | threatlockertray.exe |

### HP Client Security

| # | Process Name |
|---|-------------|
| 1 | HP.ClientSecurityManager.exe |
| 2 | HP.ClientSecurityManager.SystemInterface.exe |
| 3 | SecurityUpdateService.exe |

### Bromium (HP Sure Click)

| # | Process Name |
|---|-------------|
| 1 | Br-uxendm.exe |
| 2 | BemSvc.exe |
| 3 | BrConsole.exe |
| 4 | BrHostSvr.exe |
| 5 | BrService.exe |

### eScan (MicroWorld)

| # | Process Name |
|---|-------------|
| 1 | econser.exe |
| 2 | mwagent.exe |
| 3 | MWASER.EXE |
| 4 | consctlx.exe |
| 5 | avpmapp.exe |
| 6 | econceal.exe |
| 7 | ESERV.EXE |
| 8 | escanmon.exe |

### Google Cloud Guest Agent

| # | Process Name |
|---|-------------|
| 1 | gc-agent-ui.exe |
| 2 | gc-agents-service.exe |
| 3 | gc-enforcement-agent.exe |
| 4 | gc-guest-agent.exe |
| 5 | gc-controller.exe |
| 6 | server.exe |

### AhnLab

| # | Process Name |
|---|-------------|
| 1 | neas.exe |
| 2 | neat.exe |
| 3 | nepss64.exe |
| 4 | nepss.exe |
| 5 | nepws64.exe |
| 6 | nepws.exe |
| 7 | ASDSvc.exe |
| 8 | V3UI.exe |

---

## Targeted Kernel Drivers

### Microsoft Defender

| # | Driver Name |
|---|------------|
| 1 | WdFilter |
| 2 | MpKslDrv |
| 3 | mpsdrv |
| 4 | WdNisDrv |
| 5 | KslD |
| 6 | SgrmAgent |

### Kaspersky

| # | Driver Name |
|---|------------|
| 1 | klflt |
| 2 | klhk |
| 3 | klif |
| 4 | klips |
| 5 | KLIF.KES |
| 6 | klbackupflt.KES |
| 7 | klids |
| 8 | klupd_klif_arkmon |
| 9 | kldisk |
| 10 | klbackupdisk |
| 11 | klbackupflt |
| 12 | klgse |
| 13 | klim |
| 14 | klpd |
| 15 | klfltdev |
| 16 | klupd_klif_swmon |
| 17 | kneps |
| 18 | klupd |
| 19 | klwtp |
| 20 | klpnpflt |
| 21 | klelam |
| 22 | klupd_KES |
| 23 | klam |
| 24 | klramdisk |
| 25 | klifsdk |
| 26 | klupd_klifsdk_arkmon |

### Sophos

| # | Driver Name |
|---|------------|
| 1 | SophosED |
| 2 | sntp |
| 3 | hmpalert |
| 4 | Sophos Endpoint Defense |
| 5 | sld |
| 6 | savonaccess |
| 7 | swi_callout |

### ESET

| # | Driver Name |
|---|------------|
| 1 | epfw |
| 2 | eamonm |
| 3 | epfwwfp |
| 4 | ehdrv |
| 5 | eelam |
| 6 | ekbdflt |
| 7 | edevmon |
| 8 | em018k_64 |

### SentinelOne

| # | Driver Name |
|---|------------|
| 1 | file_monitor |
| 2 | file_protector |
| 3 | SentinelMonitor |
| 4 | SentinelDeviceControl |

### CrowdStrike

| # | Driver Name |
|---|------------|
| 1 | csagent |
| 2 | CSBoot |
| 3 | CSDeviceControl |
| 4 | CSFirmwareAnalysis |
| 5 | im.sys |

### Trend Micro

| # | Driver Name |
|---|------------|
| 1 | TmPreFilter |
| 2 | TmXPFlt |
| 3 | tmusa |
| 4 | VSApiNt |
| 5 | TmPreFlt |
| 6 | tmactmon |
| 7 | tmcomm |
| 8 | TMUMH |
| 9 | tmevtmgr |
| 10 | tmeevw |
| 11 | tmel |
| 12 | TmKmSnsr |
| 13 | TmEsFlt |
| 14 | fileflt |
| 15 | tmeyes |
| 16 | tmnciesc |
| 17 | TM_CFW |
| 18 | TMEBC |
| 19 | tmeext |
| 20 | TMLWF |
| 21 | tmtdi |
| 22 | TMWFP |
| 23 | VsapiNT |

### McAfee / Trellix

| # | Driver Name |
|---|------------|
| 1 | WFP_MRT |
| 2 | mfehidk |
| 3 | mfeplk |

### FireEye / Trellix XDR

| # | Driver Name |
|---|------------|
| 1 | FeKern |

### Symantec / Broadcom

| # | Driver Name |
|---|------------|
| 1 | BAPIDRV |
| 2 | ssfmonm |
| 3 | BHDrvx64 |
| 4 | eeCtrl64 |
| 5 | eeCtrl |
| 6 | EraserUtilRebootDrv |
| 7 | IDSvia64 |
| 8 | SRTSP64 |
| 9 | SRTSP |
| 10 | eraser |
| 11 | SRTSPIT |
| 12 | SymEvnt |
| 13 | VirtualAgent |
| 14 | pgpwdefs |
| 15 | GEProtection |
| 16 | sysMon |
| 17 | ssrfsf |
| 18 | reghook |
| 19 | spbbcdrv |
| 20 | bhdrvx86 |
| 21 | bhdrvx64 |
| 22 | SISIPSFileFilter |
| 23 | symevent |
| 24 | SYMEVENT64x86 |
| 25 | sysplant |
| 26 | diflt |
| 27 | vxfsrep |
| 28 | VirtFile |
| 29 | SymAFR |
| 30 | symefasi |
| 31 | symefa |
| 32 | symefa64 |
| 33 | SymHsm |
| 34 | evmf |
| 35 | GEFCMP |
| 36 | VFSEnc |
| 37 | pgpfs |
| 38 | fencry |
| 39 | symrg |
| 40 | vsepflt |

### Bitdefender

| # | Driver Name |
|---|------------|
| 1 | bdelam |
| 2 | Ignisv2 |
| 3 | vlflt |
| 4 | bdprivmon |
| 5 | bddci4 |
| 6 | atc |
| 7 | gemma |
| 8 | trufos |
| 9 | bdsvm |
| 10 | hbflt |
| 11 | gzflt |
| 12 | bddevflt |
| 13 | ignis |
| 14 | AVCKF |
| 15 | AVC3 |
| 16 | bddci |
| 17 | bdfsfltr |
| 18 | BdSentry |
| 19 | rtp2 |
| 20 | rtp1 |
| 21 | rtp_elam |
| 22 | BdNet |
| 23 | arwflt |
| 24 | atkldrvr |
| 25 | bdsflt |
| 26 | bsfs |
| 27 | catflt |
| 28 | dskenc |
| 29 | emlssx |
| 30 | ggc |
| 31 | kbfltr |
| 32 | snsrflt |

### Avast

| # | Driver Name |
|---|------------|
| 1 | aswSP |
| 2 | aswbuniv |
| 3 | aswbidsdriver |
| 4 | aswVmm |
| 5 | aswSnx |
| 6 | aswMonFlt |

### AVG

| # | Driver Name |
|---|------------|
| 1 | avgArPot |
| 2 | avgVmm |
| 3 | avgbuniv |
| 4 | avgSP |
| 5 | avgSnx |
| 6 | avgbidsdriver |
| 7 | avgMonFlt |

### Webroot

| # | Driver Name |
|---|------------|
| 1 | WRCore.x64 |
| 2 | WREDRD.x64 |
| 3 | WRkrn |
| 4 | WRAEKernel |
| 5 | WRCore |

### Panda Security (WatchGuard)

| # | Driver Name |
|---|------------|
| 1 | PSINProc |
| 2 | PSINFile |
| 3 | DvctProv |

### Sangfor

| # | Driver Name |
|---|------------|
| 1 | sfavflt |
| 2 | SFEhpatch |
| 3 | sfeknl |
| 4 | SFENetMon |
| 5 | sfeumsor |
| 6 | SfavBoot |
| 7 | sfwtp |
| 8 | sxfapi |
| 9 | sxfcore |
| 10 | sxfknl |

### Fortinet

| # | Driver Name |
|---|------------|
| 1 | AscFileFilter |
| 2 | Monitor_win10_x64 |
| 3 | AscRegistryFilter |
| 4 | FortiEDRWinDriver |
| 5 | FortiEDRAvDriver |
| 6 | FortiEDRBaseDriver |
| 7 | FortiEDRFsDriver |
| 8 | FortiAptFilter |
| 9 | fortimon2 |
| 10 | fortimon |
| 11 | fortishield |

### Cisco / Immunet

| # | Driver Name |
|---|------------|
| 1 | CiscoAMPCEFWDriver |
| 2 | CiscoAMPHeurDriver |
| 3 | CiscoSAM |
| 4 | ImmunetNetworkMonitor |
| 5 | immunetprotect |
| 6 | immunetselfprotect |
| 7 | ImmunetProtectDriver |
| 8 | ImmunetSelfProtectDriver |
| 9 | csaav |

### Check Point / ZoneAlarm

| # | Driver Name |
|---|------------|
| 1 | cpepmon |
| 2 | vsdatant |

### F-Secure / WithSecure

| # | Driver Name |
|---|------------|
| 1 | cbfs |
| 2 | nif2s |
| 3 | fsulgk |
| 4 | fselms |

### Qihoo 360

| # | Driver Name |
|---|------------|
| 1 | qmnetmonw64 |
| 2 | QMUdisk64_ev |
| 3 | QQSysMonX64_EV |
| 4 | TAOKernelEx64_ev |
| 5 | TFsFltX64_ev |
| 6 | TAOAcceleratorEx64_ev |
| 7 | QQSysMonX64 |
| 8 | TFsFlt |
| 9 | sysdiag_win10 |
| 10 | sysdiag |
| 11 | 360AvFlt |
| 12 | 360qpesv |
| 13 | 360AntiSteal |
| 14 | 360FsFlt |
| 15 | 360Box |
| 16 | 360netmon |
| 17 | 360AntiHacker |
| 18 | 360Hvm |
| 19 | 360AntiHijack |
| 20 | 360AntiExploit |
| 21 | DsArk |
| 22 | 360Sensor |
| 23 | 360EntSysFlt |
| 24 | 360CactusNet |

### QAX (Qi-Anxin)

| # | Driver Name |
|---|------------|
| 1 | QaxNfDrv |
| 2 | QKBaseChain64 |
| 3 | QKNetFilter |
| 4 | QKSecureIO |
| 5 | QesEngEx |
| 6 | QkHelp64 |
| 7 | qaxeng |
| 8 | qaxhook |
| 9 | QaxSysFlt |

### Huorong

| # | Driver Name |
|---|------------|
| 1 | hrwfpdrv |
| 2 | hrfwdrv |
| 3 | hrelam |
| 4 | hrdevmon |

### Antiy (AVL SDK)

| # | Driver Name |
|---|------------|
| 1 | AHipsFilter |
| 2 | AHipsFilter64 |
| 3 | GuardKrnl |
| 4 | GuardKrnl64 |
| 5 | GuardKrnlXP64 |
| 6 | protectdrv |
| 7 | protectdrv64 |
| 8 | AntiyUSB |
| 9 | AntiyUSB64 |
| 10 | AHipsXP |
| 11 | AHipsXP64 |
| 12 | AtAuxiliary |
| 13 | AtAuxiliary64 |
| 14 | TrustSrv |
| 15 | TrustSrv64 |

### Cylance (BlackBerry)

| # | Driver Name |
|---|------------|
| 1 | CyDevFlt |
| 2 | CylanceDrv |
| 3 | CyElamDrv |
| 4 | avdisk |

### ThreatLocker

| # | Driver Name |
|---|------------|
| 1 | ThreatLockerDriver |

### Bromium (HP Sure Click)

| # | Driver Name |
|---|------------|
| 1 | BrFilter |
| 2 | BrCow |

### eScan (MicroWorld)

| # | Driver Name |
|---|------------|
| 1 | ProcObsrvesx |
| 2 | mwfsmflt |
| 3 | econceal |
| 4 | ESWfp |
| 5 | MWRM |
| 6 | PROCOBSRVES |

### Google Cloud

| # | Driver Name |
|---|------------|
| 1 | gc-enforcement64 |
| 2 | gc-enforcement |

### AhnLab

| # | Driver Name |
|---|------------|
| 1 | ahnrghnt |
| 2 | AHAWKENT |
| 3 | AMonLWLH |
| 4 | ArtDrv |
| 5 | ATamptNt |
| 6 | athpexnt |
| 7 | MeDCoreD |
| 8 | MeDVpDrv |
| 9 | MeDVpHkD |
| 10 | TFFREGNT |
| 11 | TNFwNt |
| 12 | TNHipsNt |
| 13 | TNNipsNt |
| 14 | TSFltDrv |
| 15 | asc_kbc |
| 16 | AntiStealth |

### Other / Uncategorized Drivers

| # | Driver Name |
|---|------------|
| 1 | NcWpsMs |
| 2 | NcFsFltr |
| 3 | NcDxFltr |

---

## Vulnerable Drivers Used by the Killer

The EDR killer binary leverages the following **BYOVD (Bring Your Own Vulnerable Driver)** technique:

| Driver File | Service Name | Description |
|-------------|-------------|-------------|
| rwdrv.sys | mgdsrv | RWEverything driver — renamed ThrottleStop.sys (primary, physical memory R/W) |
| hlpdrv.sys | KMHLPSVC | Helper driver (secondary, process termination via IOCTL 0x2222008) |

---

## IOC Hashes (SHA256 / MD5 / SHA1)

### msimg32.dll (Malicious Loader DLL)

| Hash Type | Value |
|-----------|-------|
| **SHA256** | `7787da25451f5538766240f4a8a2846d0a589c59391e15f188aa077e8b888497` |
| MD5 | `89ee7235906f7d12737679860264feaf` |
| SHA1 | `01d00d3dd8bc8fd92dae9e04d0f076cb3158dc9c` |

### rwdrv.sys (BYOVD — RWEverything / ThrottleStop Driver)

| Hash Type | Value |
|-----------|-------|
| **SHA256** | `16f83f056177c4ec24c7e99d01ca9d9d6713bd0497eeedb777a3ffefa99c97f0` |
| MD5 | `6bc8e3505d9f51368ddf323acb6abc49` |
| SHA1 | `82ed942a52cdcf120a8919730e00ba37619661a3` |

### hlpdrv.sys (BYOVD — Process Termination Helper Driver)

| Hash Type | Value |
|-----------|-------|
| **SHA256** | `bd1f381e5a3db22e88776b7873d4d2835e9a1ec620571d2b1da0c58f81c84a56` |
| MD5 | `cf7cad39407d8cd93135be42b6bd258f` |
| SHA1 | `ce1b9909cef820e5281618a7a0099a27a70643dc` |


---

## Excluded Locales (Kill-Switch)

The binary checks for the following system locales and **does NOT execute** if any are detected (CIS country exclusion):

| Locale Code | Country |
|------------|---------|
| ru-RU | Russia |
| ru-BY | Belarus (Russian) |
| ru-KG | Kyrgyzstan (Russian) |
| ru-MD | Moldova (Russian) |
| ru-UA | Ukraine (Russian) |
| kk-KZ | Kazakhstan |
| ky-KG | Kyrgyzstan |
| uz-Cyrl | Uzbekistan (Cyrillic) |
| uz-Cyrl-UZ | Uzbekistan (Cyrillic) |
| uz-Latn | Uzbekistan (Latin) |
| uz-Latn-UZ | Uzbekistan (Latin) |
| uz-Arab | Uzbekistan (Arabic) |
| az-Cyrl | Azerbaijan (Cyrillic) |
| az-Cyrl-AZ | Azerbaijan (Cyrillic) |
| az-Latn | Azerbaijan (Latin) |
| az-Latn-AZ | Azerbaijan (Latin) |
| ka-GE | Georgia |
| uk-UA | Ukraine |
| tg-Cyrl | Tajikistan (Cyrillic) |
| tg-Cyrl-TJ | Tajikistan (Cyrillic) |
| tk-TM | Turkmenistan |
| hy-AM | Armenia |
| be-BY | Belarus |
| lt-LT | Lithuania |
| lv-LV | Latvia |
| ro-MD | Moldova |
| et-EE | Estonia |

---

## Summary Statistics

| Category | Count |
|----------|-------|
| **Total Targeted Executables** | ~198 |
| **Total Targeted Drivers** | ~286 |
| **Targeted AV/EDR Vendors** | ~30+ |
| **Vulnerable Drivers (BYOVD)** | 2 |
| **Excluded Locales** | 27 |
