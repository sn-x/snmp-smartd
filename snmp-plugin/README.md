# snmp_smartd
SMART prober and parser with SNMP persist output

## Short about

###### bin/snmp_smart

snmp-plugin packed into a single file with all perl dependencies included.

###### lib/Configurator.pm

Configuration file.

###### lib/Parser.pm

Parses smartctl output.

###### lib/Discovery.pm

Discoveres SMART capable disk drives.

###### lib/Persist.pm

Provides pass persist output.

## Dependencies:

apt: apt-get install libsnmp-extension-passpersist-perl libxml-simple-perl libfile-slurp-perl smartmontools lshw

yum: yum install

**SNMP::Extension::PassPersist**: https://metacpan.org/pod/SNMP::Extension::PassPersist

**File::Slurp**: https://metacpan.org/pod/File::Slurp

**Data::Dumper**: https://metacpan.org/pod/Data::Dumper

**XML::Simple**: https://metacpan.org/pod/XML::Simple

**lshw**: http://ezix.org/project/wiki/HardwareLiSter

**smartmontools**: https://www.smartmontools.org

## Supported features

**SMART Discovery**: JBODs, HBA/controller drivers: megaraid_sas, 3w-9xxx, aacraid, nvme, mpt2sas, ahci, isci

**SMART Parser**: Full table, Small table, Intel NVMe

**SNMP Pass Persist**

## Roadmap

- Extend discovery support for additional drivers

- Extend parser support for additional SMART outputs

