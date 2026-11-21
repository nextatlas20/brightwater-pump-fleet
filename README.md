# brightwater-pump-fleet

Condition records for the Brightwater Water Authority pumping fleet.

Every pumping station has its own long-lived branch named `station/<station id in lower case>`,
and each inspection visit is committed to `records/<inspection date>.json` on that branch.
Retired stations keep their history on an `archive/...` branch.

`standards/inspection_standard.json` on `main` carries the current inspection standard: the
measurement thresholds, the overhaul cost model and the quarterly overhaul budget.
