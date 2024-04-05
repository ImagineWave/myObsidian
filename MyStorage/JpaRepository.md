
### Список волшебных слов для заклинаний



<table>
    <tr>
        <th>------Слово-----</th>
        <th>Пример использования</th>
    </tr>
    <tr>
        <td>And</td>
        <td>findByLastnameAndFirstname</td>
    </tr>
    <tr>
        <td>Or</td>
        <td>findByLastnameOrFirstname</td>
    </tr>
    <tr>
        <td>Is, Equals</td>
        <td>findByFirstname, findByFirstnameIs, findByFirstnameEquals</td>
    </tr>
    <tr>
        <td>Between</td>
        <td>findByCreatedAtBetween (date1, date2)</td>
    </tr>
    <tr>
        <td>LessThan</td>
        <td>findByAgeLessThan</td>
    </tr>
    <tr>
        <td>LessThanEquals</td>
        <td>findByAgeLessThanEquals</td>
    </tr>
    <tr>
        <td>GreaterThan</td>
        <td>findByAgeGreaterThan</td>
    </tr>
    <tr>
        <td>GreaterThanEquals</td>
        <td>findByAgeGreaterThanEquals</td>
    </tr>
    <tr>
        <td>After</td>
        <td>findByCreatedAtAfter</td>
    </tr>
    <tr>
        <td>Before</td>
        <td>findByCreatedAtBefore</td>
    </tr>
    <tr>
        <td>isNull</td>
        <td>findByPatronymicIsNull</td>
    </tr>
    <tr>
        <td>inNotNull, NotNull</td>
        <td>findByPatronymicIsNotNull</td>
    </tr>
    <tr>
        <td>Like</td>
        <td>findByFirstnameLike(%Иван%)</td>
    </tr>
    <tr>
        <td>NotLike</td>
        <td>findByFirstnameNotLike(%Иван%)</td>
    </tr>
    <tr>
        <td>StartingWith</td>
        <td>findByFirstnameStartingWith(Иван)
        (Обертка Иван%)</td>
    </tr>    
    <tr>
        <td>EndingWith</td>
        <td>findByFirstnameEndingWith(Иван)
        (Обертка %Иван)</td>
    </tr> 
    <tr>
        <td>Containing</td>
        <td>findByFirstnameContaining(Иван)
         (Обертка %Иван%)</td>
    </tr>
    <tr>
        <td>OrderBy</td>
        <td>findAllOrderByCreatedAtDesc</td>
    </tr>
    <tr>
        <td>Not</td>
        <td>findByFirstnameNot</td>
    </tr>
    <tr>
        <td>In</td>
        <td>findByAgeIn(Collection &#60;Age&#62; age)</td>
    </tr>
    <tr>
        <td>NotIn</td>
        <td>findByAgeNotIn(Collection &#60;Age&#62; age)</td>
    </tr>
    <tr>
        <td>True</td>
        <td>findByBannedTrue</td>
    </tr>
    <tr>
        <td>False</td>
        <td>findByBannedFalse</td>
    </tr>
    <tr>
        <td>IgnoreCase</td>
        <td>findByNicknameIgnoreCase</td>
    </tr>
</table>
