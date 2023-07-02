# Getting Started

| File or Folder | Purpose                              |
| -------------- | ------------------------------------ |
| `app/`         | content for UI frontends goes here   |
| `db/`          | your domain models and data go here  |
| `srv/`         | your service models and code go here |
| `package.json` | project metadata and configuration   |
| `readme.md`    | this getting started guide           |

## Steps

1. Ensure that you create a HANA Cloud instance  
   https://hana-cockpit-001.cfapps.us10.hana.ondemand.com/hcs/sap/hana/cloud/index.html#
2. While creating the HANA Cloud trial instance, ensure that it can be accessed by 'All IP Addresses'(temporarily)
3. The HANA cloud trial instance is stopped daily so remember to restart it before deploying
4. Use 'mbt build -t gen --mtar mta.tar' to create the mtar archive
5. Deploy to cf using 'cf deploy gen/mta.tar'
6. Construct the URLs in the browser using the samples in test.http file
