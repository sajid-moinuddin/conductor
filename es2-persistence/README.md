## Usage

1. In `server/build.gradle` file,  add `compile project(':conductor-es2-persistence')` in dependencies
1. In `server/ConductorServer.java` file , replace  `import com.netflix.conductor.dao.es?.EmbeddedElasticSearch` with `import com.netflix.conductor.dao.es2.EmbeddedElasticSearch`
1. In `server/ServerModule.java` file,  replace  `import com.netflix.conductor.dao.es?.index.ElasticSearchDAO; import com.netflix.conductor.dao.es?.index.ElasticsearchModule` with `import com.netflix.conductor.dao.es2.index.ElasticSearchDAO;  import com.netflix.conductor.dao.es2.index.ElasticsearchModule;`
1. Config property 'workflow.elasticsearch.cluster.name' , value with your elasticsearch cluster name
