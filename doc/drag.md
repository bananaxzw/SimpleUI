<div class="description">
	Dragģ��ΪwebӦ��������������Ӧ�ó����Ĺ��ܺ������ԡ�Drag���������һ��DomԪ�ؿ��ƶ��� 
	���ҿ��������϶��ֱ��������϶���Ҳ���������϶��ķ�Χ��Dragģ�鱾�������һ������ģ�飬ͨ���׳����¼�ʹ�ý�����ø��Ӽ�
</div>
## ��ʼʹ��
	
	require(['ui/drag'],function(Drag){
		
		//����д������
		
	});

## demo

<div class="demo" id="demo">
	<div class="drag-demo" style="border:1px solid #979797;padding:20px 50px;width:200px;background:#fff;">
		drag me!
	</div>
</div>

���ô��룺
	
	$('.drag-demo').drag();

## Drag�ĳ�����������

����μ�<a href="http://simpleui.org/api/classes/Simple.Drag.html">API</a>

### proxy
����һ���϶�����
	
	$('.simple-dialog').drag({
		proxy:'clone'
	});
### container
�����϶��ķ�Χ
	
	$('.simple-dialog').drag({
		container:document.body
	});
	
### dropElements

<a class="btn J-dialog" href="/demo/drag.html" type="iframe">run demo</a>

ָ�����������¼���Ԫ�أ�����dom������jQueryѡ����.

* ����ж�����ö������ʱ����drop���¼���������ʹ�õ�ǰ���õ������������ȡ������Ҫʹ��ȫ�ֵ�dropElements
	
		$('#demo').drag({
			dropElements:'.test',//this element's length > 1
			listeners:{
				drop:function(dropElements){
					// not this.dropElements
					//dropElements.el do sth
				}
			}
		});
	
* ����϶���������Զ���ڷ�����������������ͬʱ������������ཻ���������һ���ཻ��������Ϊ��������

		$('.list').drag({
			//ָ���϶��ֱ�
			handle: 'h2',
			//�϶�����
			proxy: 'clone',
			//����ԭ��
			revert: true,
			//��������
			dropElements: '.drop-area',
			listeners: {
				//�϶�������
				drag: function(){
					this.dropElements.addClass('active');
				},
				//�϶�����
				dragEnter: function(){
					this.dropElements.addClass('focus');
				},
				//�϶��뿪
				dragLeave: function(){
					this.dropElements.removeClass('focus');
				},
				//�϶�ֹͣ
				dragStop: function(){
					this.dropElements.removeClass('active');
				},
				//����
				drop: function(){
					this.dropElements.find('ul').append(this.node);
					this.node.hide().fadeIn().animate({
						width: '80px',
						height: '80px'
					});
					this.dropElements.removeClass('focus');
				}
			}
		});



## �¼�
Dragģ��Ϊ�����ṩ���걸���¼�֧�֣����ϷŵĽ��������д��ø����ס�
*  `drag`���϶���ʱ�򴥷����¼�
*  `dragStart`���϶���ʼ��ʱ�򴥷����¼����������false������ֹ�϶�
*  `dragEnter`���϶��������Ԫ��ʱ�������¼�
*  `dragLeave`���϶��뿪����Ԫ��ʱ�������¼�
*  `dragStop`���϶�ֹͣ��ʱ�򴥷����¼�
*  `drop`���϶�����Ԫ��ʱ�������¼�

<script src="http://simpleui.org/demo/drag.js">
</script>

	
	
	
	



