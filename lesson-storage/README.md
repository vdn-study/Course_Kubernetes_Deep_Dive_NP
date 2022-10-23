## Recap
* Pod --> PVC --> PV --> CSI --> Storage
* CSI plays as a plugin to different storage type, sizing disk, etc.
* To make the storage dynamic, replace Storeage Class (SC) will wrap PV with configurable params depending on storage type (AWS EBS, IO, gp/io1/etc.)
