all: WellKnownServiceTypeEntry_Server.exe WellKnownServiceTypeEntry_Client.exe

WellKnownServiceTypeEntry_Server.exe: WellKnownServiceTypeEntry_Server.cs WellKnownServiceTypeEntry_Share.dll
	csc WellKnownServiceTypeEntry_Server.cs /r:WellKnownServiceTypeEntry_Share.dll

WellKnownServiceTypeEntry_Client.exe: WellKnownServiceTypeEntry_Client.cs WellKnownServiceTypeEntry_Share.dll
	csc WellKnownServiceTypeEntry_Client.cs /r:WellKnownServiceTypeEntry_Share.dll

WellKnownServiceTypeEntry_Share.dll: WellKnownServiceTypeEntry_Share.cs
	csc /t:library WellKnownServiceTypeEntry_Share.cs
