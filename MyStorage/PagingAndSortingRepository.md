

Нужно просто наследоваться от PagingAndSortingRepository

```java
public interface MyRepository extends PagingAndSortingRepository <Entity, Long>{


}
```

Умеет делать Sort'ы пагинацию итп


```java
public void testRepo{
	Iterable<Entity> allEntity = 
	myRepo.findAll(new Sort(Sort.Direction.DESC, "entityName"));

	allEntity.forEach( user ->   
    System.out.println("Пользователь "+ user.toString()));
}
```

Мы получим вывод пользователей по их полю entityName, например по login'у