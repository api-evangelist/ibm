# IBM GraphQL Schema

This directory contains a conceptual GraphQL schema for IBM Cloud and Watson AI services. The schema models the key entities, relationships, and operations exposed across IBM's REST APIs and translates them into a unified GraphQL surface.

## Coverage

The schema spans the following IBM service areas:

### IAM and Identity
Types: `Account`, `User`, `ServiceID`, `APIKey`, `Token`, `IAMPolicy`, `PolicySubject`, `PolicyRole`, `PolicyResource`, `PolicyAttribute`, `RBACRole`, `AccessGroup`, `AccessGroupMember`, `AccessGroupRule`, `AccessGroupRuleCondition`, `TrustedProfile`, `ProfileLink`

### Resource Management
Types: `ResourceGroup`, `ResourceInstance`, `ResourceKey`, `Tag`, `ServiceDefinition`, `PlanSpecification`, `Catalog`

### VPC and Networking
Types: `VPC`, `Subnet`, `Zone`, `Instance`, `Image`, `OperatingSystem`, `InstanceProfile`, `NetworkInterface`, `SecurityGroup`, `SecurityGroupRule`, `NetworkACL`, `NetworkACLRule`, `PublicGateway`, `FloatingIP`, `LoadBalancer`, `LBPool`, `LBListener`, `LBListenerPolicy`, `LBListenerPolicyRule`, `LBMember`, `LBHealthMonitor`, `Volume`, `VolumeAttachment`, `VolumeProfile`

### IBM Cloud Object Storage
Types: `COSBucket`, `BucketVersioning`, `BucketLifecycleRule`, `LifecycleTransition`, `CORSRule`, `ReplicationRule`, `ReplicationDestination`, `COSObject`

### Managed Databases
Types: `DatabaseInstance`, `DatabaseMember`, `DatabaseConnections`, `ConnectionStringSet`, `ConnectionHost`, `ConnectionCertificate`, `DatabaseBackup`, `DatabaseAutoscaling`, `AutoscalingDisk`, `AutoscalingMemory`, `AutoscalingCPU`, `DatabaseGroup`, `DatabaseGroupMembers`, `DatabaseGroupResource`

### IBM Cloudant
Types: `CloudantDatabase`, `CloudantSizes`, `CloudantCluster`, `CloudantDocument`

### IBM Event Streams (Kafka)
Types: `KafkaTopic`, `KafkaConsumerGroup`, `KafkaConsumerMember`, `KafkaConsumerOffset`

### Watson Assistant
Types: `Message`, `MessageInput`, `OutputData`, `ResponseGeneric`, `Intent`, `DialogNode`, `Context`, `ContextGlobal`, `ContextSystem`, `AssistantSession`

### Watson Natural Language Understanding
Types: `NLUResult`, `AnalyzedText`, `NLUUsage`, `ConceptsResult`, `EntitiesResult`, `EntityMention`, `EntityDisambiguation`, `KeywordsResult`, `CategoriesResult`, `CategoriesModelExplanation`, `CategoriesRelevantText`, `EmotionResult`, `DocumentEmotionResults`, `TargetedEmotionResults`, `EmotionScores`, `NLUMetadata`, `Author`, `Feed`, `RelationsResult`, `RelationArgument`, `RelationEntity`, `SemanticRolesResult`, `SemanticRolesResultSubject`, `SemanticRolesResultAction`, `SemanticRolesVerb`, `SemanticRolesResultObject`, `SentimentResult`, `SentimentScore`, `TargetedSentimentResults`, `SyntaxResult`, `SyntaxToken`, `SyntaxSentence`, `TextFeatures`, `ClassificationsOptions`, `ConceptsOptions`, `EmotionOptions`, `EntitiesOptions`, `KeywordsOptions`, `RelationsOptions`, `SemanticRolesOptions`, `SentimentOptions`, `SyntaxOptions`, `SyntaxOptionsTokens`

### Watson Speech to Text
Types: `SpeechRecognitionResult`, `SpeechRecognitionAlternativeResult`, `SpeechAlternative`, `SpeakerLabel`, `WordAlternative`, `WordAlternativeItem`, `ProcessingMetrics`, `ProcessedAudio`, `AudioMetrics`, `AudioMetricsDetails`, `AudioMetricHistogramBin`

### Watson Discovery
Types: `DiscoveryProject`, `DiscoveryCollection`, `DocumentCounts`, `DiscoveryQueryResult`, `DiscoveryDocument`, `QueryAggregation`, `AggregationResult`, `QueryResultPassage`, `ResultPassageAnswer`

### watsonx.ai
Types: `WatsonxModel`, `WatsonxModelLimits`, `WatsonxTextGenerationResult`, `WatsonxGeneratedTextResult`, `TokenInfo`, `WatsonxPrompt`, `WatsonxParameters`, `WatsonxReturnOptions`, `WatsonxEmbeddingResult`, `EmbeddingResult`

### watsonx.governance
Types: `AIFairnessMonitor`, `FairnessThreshold`, `ModelQualityMonitor`, `QualityThreshold`

### Security and Compliance
Types: `ComplianceProfile`, `ComplianceControl`, `ControlSpecification`, `Assessment`, `Parameter`, `DefaultParameter`, `EncryptionKey`, `KeyVersion`, `Secret`, `SecretVersion`

### Observability
Types: `MonitoringAlert`, `LogEntry`, `LogResource`, `ActivityTrackerEvent`, `ActivityEventReason`, `ActivityEventInitiator`, `ActivityEventTarget`

### Container Registry
Types: `ContainerRepository`, `ContainerImage`, `ImageVulnerabilityAssessment`, `ImageVulnerability`, `ConfigurationIssue`

### Code Engine (Serverless)
Types: `CodeEngineProject`, `CodeEngineApp`, `AppRevision`, `AppInstance`, `CodeEngineJob`, `JobRun`, `JobRunInstance`

### Enterprise and Billing
Types: `Enterprise`, `EnterpriseAccountGroup`, `EnterpriseAccount`, `UsageReport`, `ResourceUsage`, `PlanUsage`, `MetricUsage`

### Events
Types: `CloudEvent`

## Schema File

- [ibm-schema.graphql](ibm-schema.graphql)

## Source APIs

- https://cloud.ibm.com/apidocs (IBM Cloud API reference)
- https://cloud.ibm.com/apidocs/assistant/assistant-v2 (Watson Assistant)
- https://cloud.ibm.com/apidocs/natural-language-understanding (Watson NLU)
- https://cloud.ibm.com/apidocs/speech-to-text (Watson Speech to Text)
- https://cloud.ibm.com/apidocs/discovery-data (Watson Discovery)
- https://cloud.ibm.com/apidocs/watsonx-ai (watsonx.ai)
- https://cloud.ibm.com/apidocs/vpc/latest (IBM Cloud VPC)
- https://cloud.ibm.com/apidocs/iam-identity-token-api (IAM)
- https://cloud.ibm.com/apidocs/resource-controller/resource-controller (Resource Controller)
- https://cloud.ibm.com/apidocs/key-protect (Key Protect)
- https://cloud.ibm.com/apidocs/secrets-manager/secrets-manager-v2 (Secrets Manager)
- https://cloud.ibm.com/apidocs/security-compliance (Security and Compliance Center)
- https://cloud.ibm.com/apidocs/cloud-databases-api/cloud-databases-api-v5 (Cloud Databases)
- https://cloud.ibm.com/apidocs/cloudant (Cloudant)
- https://cloud.ibm.com/apidocs/event-streams/adminrest (Event Streams)
- https://cloud.ibm.com/apidocs/codeengine (Code Engine)
- https://cloud.ibm.com/apidocs/enterprise-apis/enterprise (Enterprise Management)
- https://github.com/IBM/ibm-cloud-sdk-common
- https://github.com/watson-developer-cloud
