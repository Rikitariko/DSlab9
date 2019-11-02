# DSlab9

## Status and configuration files.

### Primary

#### rs.status()
```
{
  "set" : "rs0",
  "date" : ISODate("2019-11-02T12:28:46.593Z"),
  "myState" : 1,
  "term" : NumberLong(1),
  "syncingTo" : "",
  "syncSourceHost" : "",
  "syncSourceId" : -1,
  "heartbeatIntervalMillis" : NumberLong(2000),
  "majorityVoteCount" : 2,
  "writeMajorityCount" : 2,
  "optimes" : {
    "lastCommittedOpTime" : {
      "ts" : Timestamp(1572697720, 1),
      "t" : NumberLong(1)
    },
    "lastCommittedWallTime" : ISODate("2019-11-02T12:28:40.741Z"),
    "readConcernMajorityOpTime" : {
      "ts" : Timestamp(1572697720, 1),
      "t" : NumberLong(1)
    },
    "readConcernMajorityWallTime" : ISODate("2019-11-02T12:28:40.741Z"),
    "appliedOpTime" : {
      "ts" : Timestamp(1572697720, 1),
      "t" : NumberLong(1)
    },
    "durableOpTime" : {
      "ts" : Timestamp(1572697720, 1),
      "t" : NumberLong(1)
    },
    "lastAppliedWallTime" : ISODate("2019-11-02T12:28:40.741Z"),
    "lastDurableWallTime" : ISODate("2019-11-02T12:28:40.741Z")
  },
  "lastStableRecoveryTimestamp" : Timestamp(1572697720, 1),
  "lastStableCheckpointTimestamp" : Timestamp(1572697720, 1),
  "electionCandidateMetrics" : {
    "lastElectionReason" : "electionTimeout",
    "lastElectionDate" : ISODate("2019-11-02T12:16:39.767Z"),
    "termAtElection" : NumberLong(1),
    "lastCommittedOpTimeAtElection" : {
      "ts" : Timestamp(0, 0),
      "t" : NumberLong(-1)
    },
    "lastSeenOpTimeAtElection" : {
      "ts" : Timestamp(1572696989, 1),
      "t" : NumberLong(-1)
    },
    "numVotesNeeded" : 2,
    "priorityAtElection" : 1,
    "electionTimeoutMillis" : NumberLong(10000),
    "numCatchUpOps" : NumberLong(27017),
    "newTermStartDate" : ISODate("2019-11-02T12:16:40.720Z"),
    "wMajorityWriteAvailabilityDate" : ISODate("2019-11-02T12:16:41.736Z")
  },
  "members" : [
    {
      "_id" : 0,
      "name" : "machine1:27017",
      "ip" : "172.31.39.234",
      "health" : 1,
      "state" : 2,
      "stateStr" : "SECONDARY",
      "uptime" : 737,
      "optime" : {
        "ts" : Timestamp(1572697720, 1),
        "t" : NumberLong(1)
      },
      "optimeDurable" : {
        "ts" : Timestamp(1572697720, 1),
        "t" : NumberLong(1)
      },
      "optimeDate" : ISODate("2019-11-02T12:28:40Z"),
      "optimeDurableDate" : ISODate("2019-11-02T12:28:40Z"),
      "lastHeartbeat" : ISODate("2019-11-02T12:28:46.173Z"),
      "lastHeartbeatRecv" : ISODate("2019-11-02T12:28:46.489Z"),
      "pingMs" : NumberLong(1),
      "lastHeartbeatMessage" : "",
      "syncingTo" : "machine2:27017",
      "syncSourceHost" : "machine2:27017",
      "syncSourceId" : 1,
      "infoMessage" : "",
      "configVersion" : 1
    },
    {
      "_id" : 1,
      "name" : "machine2:27017",
      "ip" : "172.31.0.146",
      "health" : 1,
      "state" : 1,
      "stateStr" : "PRIMARY",
      "uptime" : 821,
      "optime" : {
        "ts" : Timestamp(1572697720, 1),
        "t" : NumberLong(1)
      },
      "optimeDate" : ISODate("2019-11-02T12:28:40Z"),
      "syncingTo" : "",
      "syncSourceHost" : "",
      "syncSourceId" : -1,
      "infoMessage" : "",
      "electionTime" : Timestamp(1572696999, 1),
      "electionDate" : ISODate("2019-11-02T12:16:39Z"),
      "configVersion" : 1,
      "self" : true,
      "lastHeartbeatMessage" : ""
    },
    {
      "_id" : 2,
      "name" : "machine3:27017",
      "ip" : "172.31.26.204",
      "health" : 1,
      "state" : 2,
      "stateStr" : "SECONDARY",
      "uptime" : 737,
      "optime" : {
        "ts" : Timestamp(1572697720, 1),
        "t" : NumberLong(1)
      },
      "optimeDurable" : {
        "ts" : Timestamp(1572697720, 1),
        "t" : NumberLong(1)
      },
      "optimeDate" : ISODate("2019-11-02T12:28:40Z"),
      "optimeDurableDate" : ISODate("2019-11-02T12:28:40Z"),
      "lastHeartbeat" : ISODate("2019-11-02T12:28:46.146Z"),
      "lastHeartbeatRecv" : ISODate("2019-11-02T12:28:46.056Z"),
      "pingMs" : NumberLong(1),
      "lastHeartbeatMessage" : "",
      "syncingTo" : "machine2:27017",
      "syncSourceHost" : "machine2:27017",
      "syncSourceId" : 1,
      "infoMessage" : "",
      "configVersion" : 1
    }
  ],
  "ok" : 1,
  "$clusterTime" : {
    "clusterTime" : Timestamp(1572697720, 1),
    "signature" : {
      "hash" : BinData(0,"AAAAAAAAAAAAAAAAAAAAAAAAAAA="),
      "keyId" : NumberLong(0)
    }
  },
  "operationTime" : Timestamp(1572697720, 1)
}
```

#### rs.config()
```
{
  "_id" : "rs0",
  "version" : 1,
  "protocolVersion" : NumberLong(1),
  "writeConcernMajorityJournalDefault" : true,
  "members" : [
    {
      "_id" : 0,
      "host" : "machine1:27017",
      "arbiterOnly" : false,
      "buildIndexes" : true,
      "hidden" : false,
      "priority" : 1,
      "tags" : {
        
      },
      "slaveDelay" : NumberLong(0),
      "votes" : 1
    },
    {
      "_id" : 1,
      "host" : "machine2:27017",
      "arbiterOnly" : false,
      "buildIndexes" : true,
      "hidden" : false,
      "priority" : 1,
      "tags" : {
        
      },
      "slaveDelay" : NumberLong(0),
      "votes" : 1
    },
    {
      "_id" : 2,
      "host" : "machine3:27017",
      "arbiterOnly" : false,
      "buildIndexes" : true,
      "hidden" : false,
      "priority" : 1,
      "tags" : {
        
      },
      "slaveDelay" : NumberLong(0),
      "votes" : 1
    }
  ],
  "settings" : {
    "chainingAllowed" : true,
    "heartbeatIntervalMillis" : 2000,
    "heartbeatTimeoutSecs" : 10,
    "electionTimeoutMillis" : 10000,
    "catchUpTimeoutMillis" : -1,
    "catchUpTakeoverDelayMillis" : 30000,
    "getLastErrorModes" : {
      
    },
    "getLastErrorDefaults" : {
      "w" : 1,
      "wtimeout" : 0
    },
    "replicaSetId" : ObjectId("5dbd739c661f71bbeba6cdc5")
  }
}
```

### Secondary
#### rs.status()
```
{
  "set" : "rs0",
  "date" : ISODate("2019-11-02T12:27:21.748Z"),
  "myState" : 2,
  "term" : NumberLong(1),
  "syncingTo" : "machine2:27017",
  "syncSourceHost" : "machine2:27017",
  "syncSourceId" : 1,
  "heartbeatIntervalMillis" : NumberLong(2000),
  "majorityVoteCount" : 2,
  "writeMajorityCount" : 2,
  "optimes" : {
    "lastCommittedOpTime" : {
      "ts" : Timestamp(1572697640, 1),
      "t" : NumberLong(1)
    },
    "lastCommittedWallTime" : ISODate("2019-11-02T12:27:20.738Z"),
    "readConcernMajorityOpTime" : {
      "ts" : Timestamp(1572697640, 1),
      "t" : NumberLong(1)
    },
    "readConcernMajorityWallTime" : ISODate("2019-11-02T12:27:20.738Z"),
    "appliedOpTime" : {
      "ts" : Timestamp(1572697640, 1),
      "t" : NumberLong(1)
    },
    "durableOpTime" : {
      "ts" : Timestamp(1572697640, 1),
      "t" : NumberLong(1)
    },
    "lastAppliedWallTime" : ISODate("2019-11-02T12:27:20.738Z"),
    "lastDurableWallTime" : ISODate("2019-11-02T12:27:20.738Z")
  },
  "lastStableRecoveryTimestamp" : Timestamp(1572697600, 1),
  "lastStableCheckpointTimestamp" : Timestamp(1572697600, 1),
  "members" : [
    {
      "_id" : 0,
      "name" : "machine1:27017",
      "ip" : "172.31.39.234",
      "health" : 1,
      "state" : 2,
      "stateStr" : "SECONDARY",
      "uptime" : 652,
      "optime" : {
        "ts" : Timestamp(1572697630, 1),
        "t" : NumberLong(1)
      },
      "optimeDurable" : {
        "ts" : Timestamp(1572697630, 1),
        "t" : NumberLong(1)
      },
      "optimeDate" : ISODate("2019-11-02T12:27:10Z"),
      "optimeDurableDate" : ISODate("2019-11-02T12:27:10Z"),
      "lastHeartbeat" : ISODate("2019-11-02T12:27:20.012Z"),
      "lastHeartbeatRecv" : ISODate("2019-11-02T12:27:20.427Z"),
      "pingMs" : NumberLong(0),
      "lastHeartbeatMessage" : "",
      "syncingTo" : "machine2:27017",
      "syncSourceHost" : "machine2:27017",
      "syncSourceId" : 1,
      "infoMessage" : "",
      "configVersion" : 1
    },
    {
      "_id" : 1,
      "name" : "machine2:27017",
      "ip" : "172.31.0.146",
      "health" : 1,
      "state" : 1,
      "stateStr" : "PRIMARY",
      "uptime" : 652,
      "optime" : {
        "ts" : Timestamp(1572697630, 1),
        "t" : NumberLong(1)
      },
      "optimeDurable" : {
        "ts" : Timestamp(1572697630, 1),
        "t" : NumberLong(1)
      },
      "optimeDate" : ISODate("2019-11-02T12:27:10Z"),
      "optimeDurableDate" : ISODate("2019-11-02T12:27:10Z"),
      "lastHeartbeat" : ISODate("2019-11-02T12:27:20.016Z"),
      "lastHeartbeatRecv" : ISODate("2019-11-02T12:27:20.108Z"),
      "pingMs" : NumberLong(1),
      "lastHeartbeatMessage" : "",
      "syncingTo" : "",
      "syncSourceHost" : "",
      "syncSourceId" : -1,
      "infoMessage" : "",
      "electionTime" : Timestamp(1572696999, 1),
      "electionDate" : ISODate("2019-11-02T12:16:39Z"),
      "configVersion" : 1
    },
    {
      "_id" : 2,
      "name" : "machine3:27017",
      "ip" : "172.31.26.204",
      "health" : 1,
      "state" : 2,
      "stateStr" : "SECONDARY",
      "uptime" : 723,
      "optime" : {
        "ts" : Timestamp(1572697640, 1),
        "t" : NumberLong(1)
      },
      "optimeDate" : ISODate("2019-11-02T12:27:20Z"),
      "syncingTo" : "machine2:27017",
      "syncSourceHost" : "machine2:27017",
      "syncSourceId" : 1,
      "infoMessage" : "",
      "configVersion" : 1,
      "self" : true,
      "lastHeartbeatMessage" : ""
    }
  ],
  "ok" : 1,
  "$clusterTime" : {
    "clusterTime" : Timestamp(1572697640, 1),
    "signature" : {
      "hash" : BinData(0,"AAAAAAAAAAAAAAAAAAAAAAAAAAA="),
      "keyId" : NumberLong(0)
    }
  },
  "operationTime" : Timestamp(1572697640, 1)
}
```

#### rs.config()
```
{
  "_id" : "rs0",
  "version" : 1,
  "protocolVersion" : NumberLong(1),
  "writeConcernMajorityJournalDefault" : true,
  "members" : [
    {
      "_id" : 0,
      "host" : "machine1:27017",
      "arbiterOnly" : false,
      "buildIndexes" : true,
      "hidden" : false,
      "priority" : 1,
      "tags" : {
        
      },
      "slaveDelay" : NumberLong(0),
      "votes" : 1
    },
    {
      "_id" : 1,
      "host" : "machine2:27017",
      "arbiterOnly" : false,
      "buildIndexes" : true,
      "hidden" : false,
      "priority" : 1,
      "tags" : {
        
      },
      "slaveDelay" : NumberLong(0),
      "votes" : 1
    },
    {
      "_id" : 2,
      "host" : "machine3:27017",
      "arbiterOnly" : false,
      "buildIndexes" : true,
      "hidden" : false,
      "priority" : 1,
      "tags" : {
        
      },
      "slaveDelay" : NumberLong(0),
      "votes" : 1
    }
  ],
  "settings" : {
    "chainingAllowed" : true,
    "heartbeatIntervalMillis" : 2000,
    "heartbeatTimeoutSecs" : 10,
    "electionTimeoutMillis" : 10000,
    "catchUpTimeoutMillis" : -1,
    "catchUpTakeoverDelayMillis" : 30000,
    "getLastErrorModes" : {
      
    },
    "getLastErrorDefaults" : {
      "w" : 1,
      "wtimeout" : 0
    },
    "replicaSetId" : ObjectId("5dbd739c661f71bbeba6cdc5")
  }
}
```

## Screenshot of application.
![Chat]()
