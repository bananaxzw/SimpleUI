<div class="description">
	Menuģ��ΪwebӦ�ó����ṩ�������˵��Ĺ��ܣ�Menu�������κ�ģ�����׵�����������Ҫ�Ĺ��ܡ�Menuģ����������ࣺ
	Menu��ContextMenu,����ContextMenu��Menu�����࣬ΪwebӦ���ṩ�Ҽ��˵��Ĺ��ܡ�
</div>
## ��ʼʹ��

������Ҫ����menuģ��
	
	require(['ui/menu'],function(Menu){
		
		//����д������
		
	});

## demo

<a class="J-dialog btn" href="/demo/menu.html">run demo</a>

���ô��룺
	
	$('#button').menu({
		items:[{label:'i menu',url:'http://simpleui.org'}]
	});

## Menu���ܵ����ݸ�ʽ

����μ�<a href="http://simpleui.org/api/classes/Simple.Menu.html">API</a>

Menu����������ֲ�ͬ�����ݸ�ʽ����Ⱦ��ͬ�Ĳ˵�.�ܱ�ǸMenu������֧�ֵ����������ʽ�����ݣ���������ĸ�ʽ�ǲ���֧�ֵ�

	['menu1','menu2','men3']
	
��Ϊ��������������Ⱦ����Ҳû���κ����壬û���¼���û��������ת�������������ύ�������ݵ�����һ��.

### ��ͨ�˵�

	[{
		label:'menu',
		url:'http://baidu.com'
	}]

### ����˵�

	[{
		title: 'Menu Title',
		items: [{
		
			label: 'i menu',
			event: function(){},
			checked: true,
		   
		}]
	}]
	
### �༶�˵�
	
	[{
		title: 'Menu Title',
		items: [{
		
			label: 'i menu',
			event: function(){},
			checked: true,
		    childs:[{
				label: 'i menu'
			}]
		}]
	}]


## Menu�ĳ��÷���

### addChild

����Ѵ��ڵĲ˵����ѡ��������ܵ����ݸ�ʽͬ�ϡ�

### getItem

��ȡ���е�menuItem��ʵ��

	menu.getItem(1).set('checked',true);

## �Ҽ��˵�

	$('#button').contextmenu({
		items:[{label:'i menu',url:'http://simpleui.org'}]
	});


<script src="http://simpleui.org/demo/menu.js">
</script>

	
	
	
	



