## bootstrap table

Simple table for bootstrap. [Examples and documentation](http://wenzhixin.net.cn/p/bootstrap-table/)

### How to use:

	$('#table').bootstrapTable({
		columns: [
			{field: 'code', title: 'Code', align: 'left', width: 200},
			{field: 'name', title: 'Name', align: 'center', width: 100},
			{field: 'price', title: 'Price', align: 'right', width: 200, formatter: function(value, row) {
				return 'the price is: ' + value;
			}}
		],
		data: [
			{code: '123', name: 'hello 123', price: '$123'},
			{code: '222', name: 'hello 222', price: '$222'},
			{code: '321', name: 'hello 321', price: '$321'}
		]
	});
	
	$('#table').bootstrapTable('load', [
		{code: '123', name: 'hello 123', price: '$123'},
		{code: '222', name: 'hello 222', price: '$222'},
		{code: '321', name: 'hello 321', price: '$321'}
	]);
	
	$('#table').bootstrapTable('append', [
		{code: '123', name: 'hello 123', price: '$123'},
		{code: '222', name: 'hello 222', price: '$222'},
		{code: '321', name: 'hello 321', price: '$321'}
	]);
	