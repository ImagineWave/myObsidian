### Репозитории :
 * ##### [[CrudRepository]]
 * ##### [[PagingAndSortingRepository]]
 * ##### [[JpaRepository]]
 * #### MongoRepository
 * #### Neo4jRepository
 * #### SipleCassandraRepository

### Использование через наследование интерфейса

```java
@Repository
public interface ServerRepository extends JpaRepository<Server, Integer> {  
    // возвращает все серверы из базы  
    public List<Server> findAll();  
  
    // возвращает весь список сервепров с заданными параметрами  
    public Page<Server> findAll(final Pageable pageable);  
  
    // возвращает сервер по заданному имени  
    public Server findFirstByServerName(final String serverName);  
}
```

Я унаследовал свой интерфейс репозиторий от [[JpaRepository]]
```java
extends JpaRepository<Server, Integer>
```

### Использование через аннотацию [[@RepositoryDefenition]]

```java
  
@RepositoryDefinition( domainClass = Server.class, idClass = Integer.class)  
public interface ServerRepository {  

    // возвращает сервер по заданному имени без учета регистра
    public Server findFirstByServerNameIgnoreCase(final String serverName);  
}
```

В таком случае, в репозитории не будет НИЧЕГО КРОМЕ объявленных в нем методов. В этом случае у нас также работают [[JpaRepository | заклинания]]
