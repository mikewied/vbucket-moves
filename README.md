
vbucket-moves.py is a tool that analyzes a master events file from Couchbase Server. The master events file shows rebalance events and can be obtained at http://hostname:8091/diag/masterEvents. You will need to authenticate to get the file.

The ouput of this tool is a gantt chart of vbucket movements which show how long it took to move each vbucket. It also displays information about how long backfill takes, how long it takes to persist all backfill items, and how long it takes to index all of the items.

To run the tool type the following:

./vbucket-moves