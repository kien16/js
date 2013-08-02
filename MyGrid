Ext.define('Ext.MyGrid', {
    extend: 'Ext.grid.Panel',
    alias: 'widget.mygrid',  
	width:500,
	height:180,
	stripeRows: true,
	store: Ext.create('Ext.data.ArrayStore', {
		fields: [
			{name: 'id', type: 'int'},
			{name: 'name'},
			{name: 'position'},
			{name: 'ambition'}
		],
		data: [
			[1,'Monkey D Luffy','Captain','I will become the pirate king'],
			[2,'Roronoa Zoro','Swordman','Become the greatest swordman'],
			[3,'Sanji','Cook','Find all blue'],
			[4,'Usopp','Sniper','Become the greatest warrior'],
			[5,'Nami','Navigator','Draw map of the world']
		]
	}),
	columns: [
		{id:'id',header: 'ID', width: 30, sortable: true, dataIndex: 'id'},
		{header: 'Name', width: 100, dataIndex: 'name'},
		{header: 'Position', width: 100, dataIndex: 'position'},
		{header: 'Ambition', width: 250, dataIndex: 'ambition'}
	],
	listeners : {
		itemclick: function (grid, record, item, index, e, eOpts ) {
			// How to return some value to outside
      var variable = record.data.name;
      alert(variable);
			this.up('window').close();
		}
	}
});
