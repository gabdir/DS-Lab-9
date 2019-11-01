# DS-Lab-9

rs.status()
rs0:PRIMARY> rs.status()
{
	"set" : "rs0",
	"date" : ISODate("2019-10-29T16:27:08.610Z"),
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
			"ts" : Timestamp(1572366420, 1),
			"t" : NumberLong(1)
		},
		"lastCommittedWallTime" : ISODate("2019-10-29T16:27:00.945Z"),
		"readConcernMajorityOpTime" : {
			"ts" : Timestamp(1572366420, 1),
			"t" : NumberLong(1)
		},
		"readConcernMajorityWallTime" : ISODate("2019-10-29T16:27:00.945Z"),
		"appliedOpTime" : {
			"ts" : Timestamp(1572366420, 1),
			"t" : NumberLong(1)
		},
		"durableOpTime" : {
			"ts" : Timestamp(1572366420, 1),
			"t" : NumberLong(1)
		},
		"lastAppliedWallTime" : ISODate("2019-10-29T16:27:00.945Z"),
		"lastDurableWallTime" : ISODate("2019-10-29T16:27:00.945Z")
	},
	"lastStableRecoveryTimestamp" : Timestamp(1572366390, 1),
	"lastStableCheckpointTimestamp" : Timestamp(1572366390, 1),
	"electionCandidateMetrics" : {
		"lastElectionReason" : "electionTimeout",
		"lastElectionDate" : ISODate("2019-10-29T14:13:29.698Z"),
		"termAtElection" : NumberLong(1),
		"lastCommittedOpTimeAtElection" : {
			"ts" : Timestamp(0, 0),
			"t" : NumberLong(-1)
		},
		"lastSeenOpTimeAtElection" : {
			"ts" : Timestamp(1572358398, 1),
			"t" : NumberLong(-1)
		},
		"numVotesNeeded" : 2,
		"priorityAtElection" : 1,
		"electionTimeoutMillis" : NumberLong(10000),
		"numCatchUpOps" : NumberLong(27017),
		"newTermStartDate" : ISODate("2019-10-29T14:13:30.722Z"),
		"wMajorityWriteAvailabilityDate" : ISODate("2019-10-29T14:13:31.605Z")
	},
	"members" : [
		{
			"_id" : 0,
			"name" : "m1:27017",
			"ip" : "172.31.21.171",
			"health" : 1,
			"state" : 1,
			"stateStr" : "PRIMARY",
			"uptime" : 8093,
			"optime" : {
				"ts" : Timestamp(1572366420, 1),
				"t" : NumberLong(1)
			},
			"optimeDate" : ISODate("2019-10-29T16:27:00Z"),
			"syncingTo" : "",
			"syncSourceHost" : "",
			"syncSourceId" : -1,
			"infoMessage" : "",
			"electionTime" : Timestamp(1572358409, 1),
			"electionDate" : ISODate("2019-10-29T14:13:29Z"),
			"configVersion" : 1,
			"self" : true,
			"lastHeartbeatMessage" : ""
		},
		{
			"_id" : 1,
			"name" : "m2:27017",
			"ip" : "172.31.30.115",
			"health" : 1,
			"state" : 2,
			"stateStr" : "SECONDARY",
			"uptime" : 8029,
			"optime" : {
				"ts" : Timestamp(1572366420, 1),
				"t" : NumberLong(1)
			},
			"optimeDurable" : {
				"ts" : Timestamp(1572366420, 1),
				"t" : NumberLong(1)
			},
			"optimeDate" : ISODate("2019-10-29T16:27:00Z"),
			"optimeDurableDate" : ISODate("2019-10-29T16:27:00Z"),
			"lastHeartbeat" : ISODate("2019-10-29T16:27:08.157Z"),
			"lastHeartbeatRecv" : ISODate("2019-10-29T16:27:07.813Z"),
			"pingMs" : NumberLong(1),
			"lastHeartbeatMessage" : "",
			"syncingTo" : "db1:27017",
			"syncSourceHost" : "db1:27017",
			"syncSourceId" : 0,
			"infoMessage" : "",
			"configVersion" : 1
		},
		{
			"_id" : 2,
			"name" : "m3:27017",
			"ip" : "172.31.28.68",
			"health" : 1,
			"state" : 2,
			"stateStr" : "SECONDARY",
			"uptime" : 8029,
			"optime" : {
				"ts" : Timestamp(1572366420, 1),
				"t" : NumberLong(1)
			},
			"optimeDurable" : {
				"ts" : Timestamp(1572366420, 1),
				"t" : NumberLong(1)
			},
			"optimeDate" : ISODate("2019-10-29T16:27:00Z"),
			"optimeDurableDate" : ISODate("2019-10-29T16:27:00Z"),
			"lastHeartbeat" : ISODate("2019-10-29T16:27:08.217Z"),
			"lastHeartbeatRecv" : ISODate("2019-10-29T16:27:07.903Z"),
			"pingMs" : NumberLong(1),
			"lastHeartbeatMessage" : "",
			"syncingTo" : "m1:27017",
			"syncSourceHost" : "m1:27017",
			"syncSourceId" : 0,
			"infoMessage" : "",
			"configVersion" : 1
		}
	],
	"ok" : 1,
	"$clusterTime" : {
		"clusterTime" : Timestamp(1572366420, 1),
		"signature" : {
			"hash" : BinData(0,"AAAAAAAAAAAAAAAAAAAAAAAAAAA="),
			"keyId" : NumberLong(0)
		}
	},
	"operationTime" : Timestamp(1572366420, 1)
}
