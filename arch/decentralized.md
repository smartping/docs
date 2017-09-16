#去中心化设计

去中心化设计是SmartPing的一大特点，这里的去中心化并非集群概念，而是与分布式更加接近，简单点理解及数据分布式存储，各节点通过互相调用保持数据展示的统一性。

## 实例

如在我们的网络中存在三个对等节点A，B，C；三个节点之间将产生3!(3*2*1)=6条交互数据，在SmartPing中，每个节点存储相同的配置数据(Conf)，检测数据只存储目标为其他节点的数据，及A存储 A->B|A->C , B存储B->C|B-A，C存储C->A|C->B的数据， 当用户访问任意一个节点时，用户在前端进行各节点的数据汇总使各节点的数据展示在前端上保持一致。

![](/assets/decenter.png)