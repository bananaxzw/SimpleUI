<div class="description">
	PaginationΪwebҳ���ṩ��ҳ���ܣ���ͳ��ҳ���ҳһ�㶼�Ǻ�����ɵģ����Ƕ�����ˢ�µ����ݽ������ԣ���ҳ��������ǰ�����ɵġ�
	�����κδ����������ݻ����ӳټ��ص����ݣ���ҳչʾ���ǱȽϳ�������Ϊ��
</div>
<div class="notes">
	Paginationû���ṩ���Ӧ��jQuery������ԭ������Ϊ����Pagination����û����ȷ��node�ڵ�,��������������
</div>
## ��ʼʹ��

������Ҫ����paginationģ��
	
	require(['ui/pagination'],function(Pagination){
		
		//����д������
		
	});

## demo

<div class="demo" id="demo">
	
</div>

	new Pagination({
		container:'#demo'
	});

## ��ҳ����

�ڷ�ҳ�����ָ��pageStyle���Զ��Ʒ�ҳ����ʽ�������Ҫ��ͬ�ķ�ҳ��ʽ���Pagination.style��Ӳ�ͬ�ķ������ɡ�
	
	Pagination.style.simple = function(currentPage,totalPage){
		
		//��װHTML������
		
		return pageHtml;
	}


## ����

* `set` ���õ�ǰҳ������ҳ�����߷�ҳ�ߴ�,`currentPage`,`pageSize`,`totalCount`.

		var pagination = new Pagination({
			container:'#demo',
			listeners:{
				currentPageChange:function(){
					console.log(this.currentPage);
				}
			}
		});

		pagination.set('currentPage',2);
		pagination.set('pageSize',10);
	
## �¼�

* `beforeCurrentPageChange`��ͨ�����¼�����ֹ��ǰҳ�ĸı�
* `currentPageChange`��ͨ�����¼�������ǰҳ�ĸı�

<script src="http://simpleui.org/demo/pagination.js">
</script>

	
	
	
	



