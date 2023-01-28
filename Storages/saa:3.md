**SAA-C03**

A.

1. Warm StandBy: This solution meets the requirement for an RTO of 5 minutes. The instances run at a low capacity and can scale within minutes.
2. Pilot light
3. Multi-site active-active
4. Backup and Restore

B.

1. SSD-Backed Storage Optimized (i2) instances provide more than 365,000 random IOPS. The instance store has no additional cost, compared with the regular hourly cost of the instance. For more information about i2 storage, see[Instance store volumes](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/InstanceStorage.html#instance-store-volumes).For more information about pricing for EC2 instances, see [Amazon EC2 pricing](https://aws.amazon.com/ec2/pricing/).

    2.	Provisioned IOPS SSD (io1 or io2) EBS volumes can deliver more than the 40,000 IOPS that are required in the scenario. However, this 		     solution is not as cost-effective as an instance store because Amazon EBS adds cost to the hourly instance rate. This solution provides   persistence of data beyond the lifecycle of the instance, but persistence is not required in this use case.For more information about Provisioned IOPS SSD (io1 or io2) EBS volumes, see[Provisioned IOPS SSD volumes](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-volume-types.html#EBSVolumeTypes_piops). For more information about pricing for Amazon EBS, see [Amazon EBS pricing](https://aws.amazon.com/ebs/pricing/).

3. Throughput Optimized HDD (st1) EBS volumes are engineered to maximize the throughput of data that can be sent to and from a volume, not the random IOPS. Consequently, this solution does not meet the IOPS requirement. In addition, Amazon EBS adds cost to the hourly instance rate. This solution provides persistence of data beyond the lifecycle of the instance, but persistence is not required in this use case. For more information about Throughput Optimized HDD (st1) EBS volumes, see [Throughput Optimized HDD volumes](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-volume-types.html#EBSVolumeTypes_st1).For more information about pricing for Amazon EBS, see [Amazon EBS pricing](https://aws.amazon.com/ebs/pricing/).
4. The rapidly changing data that is required for the scratch volume space makes Amazon S3 (object storage) the wrong storage. Block storage is appropriate for the read/write functionality to work smoothly. For more information about usage patterns for Amazon S3, see [Performance Design Patterns for Amazon S3](https://docs.aws.amazon.com/AmazonS3/latest/userguide/optimizing-performance-design-patterns.html).
