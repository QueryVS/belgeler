# System Design Belgeler

System Design, yazılımın diğer servislerle etkileşimini gösteren yerine göre ayrıntılı veya ayrıntı olmadan yazılımın bileşenlerinin birbirleri ile nasıl etkileşimde olduğunu gösteren şema'lardır. Bir microservice'in aralarında nasıl etkileşimde bulunduğunu, micoservice'lerin database,cahce,cdn,dns,api gateway,... gibi bileşenlerin nasıl etkileşimde olduğunu hangi region'larda ve zone'larda bulunduğunu söyleyebilirler. 

**System Design** , aşaması bir projeye başlamanın ilk aşamalarından birisidir. Projenin özellikleri, amacı, olası ölçeği, ne kadar yük kaldırması gerektiği, ne kadar High Availability olacağı, latency süreleri, güvenlik konusunda ne kadar ileri gidileceği ve multi region erişimin olup olmayacağı belirlenir.

System Design yaparken bazı parametrelerin olup olmayacağı varsayılarak tasarlanabilir veya sadece bir mikroservisin veya modül için system design yapılabilir. Belli problemleri çözmek için kullanılmış ve büyük şirketler tarafından yayınlanmış System Design'larını inceleyerek kendi probleminizde benzer bir mimari kullanabilirmisiniz. Bu tür veriler büyük şirketler tarafından yayınlanabilmektedir. 

Bu belgede system design konusunun ilgili olduğu konuları kapsayacak şekilde hazırladım. 

 - [Terminology](terminology.md)
   - Distributed Systems Properties
     - Scalability
     - Availability
     - Reliability
     - Consistency
     - Partition Tolerance
     - Fault Tolerance
     - Performance
     - Latency
     - Throughput
     - Security
     - Privacy
     - Caching
     - Auditing
     - Load Balancing
     - Data Partitioning
     - Data Replication
     - Message Queuing
     - Request-Response Communication
     - Publish-Subscribe Communication
     - Leader Election
 - [Theorems](theorems.md)
   - CAP theorem
   - BASE theorem
   - FLP theorem
   - Brewer and Nash theorem
   - Gilbert ve Lynch theorem
   - Brewer theorem
   - Gilbert and Lynch's PACELC theorem
   - Brewer's CAP theorem
   - FLP impossibility theorem
   - Brewer and Nash's theorem
   - Leslie Lamport's Byzantine fault tolerance theorem
   - Eric Brewer's Gossip protocol theorem
 - [Algorithms](algorithms.md)
   - Leader Election
     - Bully
     - Ring
     - Paxos
     - Raft
     - Zab
   - Load Balancing
     - Round Robin
     - Least Connection
     - IP Hash
     - Random
     - Weighted Round Robin
     - Weighted Least Connection
   - Consensus
     - Paxos
     - Raft
     - Zab
   - Gossip
   - MapReduce
   - Byzantine Fault Tolerance
     - PBFT
     - Tendermint
     - Algorand 
     - Bitcoin Core
 - [Best Problems](best_problems.md)