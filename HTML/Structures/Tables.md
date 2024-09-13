```html
<thead> <!-- encapsulates the table header-->
	<tr>
		<th scope="col">Table header, the scope can be col (column) or row</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data</td> <!-- <tr> = table row <td> tabledata-->
		<td colspan="2">This data will span 2 columns</td>
		<td rowspan="2"></td>This data will span 2 rows</td>
	</tr>
</tbody>
<tr>
	<tfoot>
		<td>This is a footer</td>
	</tfoot>
</tr>
```