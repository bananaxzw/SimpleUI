<div class="description">
	Button���ṩ���������水ť�Ĺ��ܣ���Ȼԭ��HTMLԪ�ذ���button�����Ƕ���һЩ��Ӧ�ã�button������Ҫ���Ƶġ�
	Buttonģ����������ࣺButton,DropDownButton,ComboButton������DropButton��ComboButton�̳���Button
</div>
## ��ʼʹ��
	
	require(['ui/button'],function(Button){
		
		//����д������
		
	});

## demo--һ����ͨ�İ�ť

<div class="demo" id="demo">
	
</div>

���ô��룺
	
	new Button({
		container:'#demo'
	});
	
## demo--һ��������ť

<div class="demo" id="demo2">
	
</div>

���ô��룺
	
	var menu = new Simple.Menu({
		items:[{label:'simple-menu'}]
	})
	new Simple.DropDownButton({
		container:'#demo',
		dropdown:menu
	});
	
## Button�ĳ��÷���

* `set`,�÷�����Attribute�̳ж�������������һЩ����,Ŀǰ֧�ֿ����õĲ����У�
** label,icon,disabled

�ı�Button�����Լȿ���ͨ���ڳ�ʼ���Ĵ��������Ҳ������ʵ������ɺ��ֶ�����set�������ﵽͬ����Ŀ�ġ�

### ���ð�ť
	
	var button = new Button({
		disabled:true
	})
	//����������Ĵ���
	var button = new Button();
	button.set('disabled',true);
	
### ���ð�ť

	button.set('disabled',false);

## ����

	button.destroy();

<script src="http://simpleui.org/demo/button.js">

</script>

	
	
	
	



