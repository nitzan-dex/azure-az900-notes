### Compare Azure storage services
The Azure Storage platform offers several services, all of which are accessible by HTTP/HTTPS and client libraries, and encrypt the data their storing.  

1. Blob storage: massive amounts of unstructured data
2. Azure Files: file shares accessible via SMB or NFS
3. Queue storage: for messages.
4. Disk storage: disk storage for Azure VMs.
5. Table Storage: structured NoSQL data (schemaless)

### Describe storage tiers
Storage tiers are configuration parameters you can define at the resource or account level that indicate the frequency with which you access your data.  
- Hot: frequent access..
- Cool: storage accessed roughly once a month.  
- Cold: storage accessed roughly once every 90 days.  
- Archive: storage accessed roughly once a year. highest cost for reads.  

### Describe redundancy options
1. Locally Redudant (LRS): Three copies in a single data center.
2. Zone Redundant (ZRS): Replicated across three AZ.
3. Geo-redundant (GRS): LRS in two data centers that are in region pairs.
4. Geo-zone Redundant (GZRS): ZRS in the primary region and LRS in secondary region.  
5. Read-Access GRS, Read-Access GZRS: Allows reads from secondary region even if primary region is up and running.  

### Describe storage account options and storage types
- Standard General-Purpose v2: Supports blobs, files, queues, tables. Redundancy: All.
- Premium Block Blobs: High transaction rates, low latency. Supports block blobs, append blobs. Redundancy: LRS, ZRS.
- Premium File Shares: High performance,SMB, NFS. Redundancy: LRS, ZRS.
- Premium Page Blobs: Optimized for page blobs. Redundancy: LRS, ZRS.

### Identify options for moving files, including AzCopy, Azure Storage Explorer, and Azure File Sync
**AzCopy** is a command-line tool for moving files locally, between storage accounts, and across cloud providers. It also supports file sync from a source to a target location.

**Azure Storage Explorer** GUI For AzCopy

**Azure File Sync** installed locally for bi-directional file sync.

### Describe migration options, including Azure Migrate and Azure Data Box
**Azure Migrate** assesses and performs network migrations.
**Azure Data Box** handles offline data migrations, ideal for over 40TB with limited network capabilities, using a physical hard drive sent to a data center.
