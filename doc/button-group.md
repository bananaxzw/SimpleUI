<div class="description">
	ButtonGroup��Button�ļ��ϣ������ṩ�����ݣ���Ⱦ���Button��������Ҫ�ܶఴťʱ�ǳ����ã����ҿ��Ը���������ѡ��۽����߽������������ĳ����ť��
	
</div>
## ��ʼʹ��
	
	require(['ui/button-group'],function(ButtonGroup){
		
		//����д������
		
	});

## demo

<div class="demo" id="demo-btn-group">
	
</div>

���ô��룺
	
	new Button({
		items : {
			'index1' : function () {
				console.log('index1');
			},
			'index2' : function () {
				console.log('index2');
			}
		},
		container : '#demo-btn-group'
	});

## ButtonGroup�ĳ��÷���



�ı�Button�����Լȿ���ͨ���ڳ�ʼ���Ĵ��������Ҳ������ʵ������ɺ��ֶ�����set�������ﵽͬ����Ŀ�ġ�

### ���ð�ť
	
	button.disable(1);
	
### ���ð�ť

	button.enable(1);

## ����

	button.destroy();

<script src="http://simpleui.org/demo/button.js">

</script>

	
	
	
	



