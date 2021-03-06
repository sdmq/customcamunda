# 流程引擎Camunda 解析说明			

Camunda流程引擎，2003年Fork自Activiti，逐渐的发展为有自己的特色的一款高效，易用，嵌入式的引擎。      
---   

1. camunda提供一个免费的BPMN2.0的构建工具：Camunda Modeler：[具体的下载地址](https://camunda.com/download/modeler/)       
  
2. 为了检验如何增加扩展功能，自定义CustomRepositoryService服务：[具体的配置见](https://github.com/AndiHappy/customcamunda/wiki/%E6%89%A9%E5%B1%95%E6%88%96%E4%BF%AE%E6%94%B9%E5%BC%95%E6%93%8E%E5%8A%9F%E8%83%BD)                 
3. camunda已经能够支持直接构建bpmnModel，所以直接使用：Bpmn.readModelFromStream 来校验BPMN文件的正确性       
4. 确认Service task的配置，代理类的用法:[具体的实现逻辑](https://github.com/AndiHappy/customcamunda/wiki/%E5%89%8D%E5%8A%A0%E7%AD%BE%EF%BC%8C%E5%90%8E%E5%8A%A0%E7%AD%BE%E7%9A%84%E5%AE%9E%E7%8E%B0)         
5. 扩展流程引擎支持的加签操作：[具体的扩展实现](https://github.com/AndiHappy/customcamunda/wiki/%E5%89%8D%E5%8A%A0%E7%AD%BE%EF%BC%8C%E5%90%8E%E5%8A%A0%E7%AD%BE%E7%9A%84%E5%AE%9E%E7%8E%B0)     
6. 扩展流程引擎支持驳回操作:[驳回操作实现](https://github.com/AndiHappy/customcamunda/wiki/%E9%A9%B3%E5%9B%9E%E5%8A%9F%E8%83%BD%E6%94%AF%E6%8C%81%E5%AE%8C%E6%88%90)     
7. 流程中任务的串并行和多实例:[具体的实现和介绍](https://github.com/AndiHappy/customcamunda/wiki/%E4%BB%BB%E5%8A%A1%E7%9A%84%E5%A4%9A%E5%AE%9E%E4%BE%8B%E5%92%8C%E4%B8%B2%E5%B9%B6%E8%A1%8C)   [具体的测试流程和代码](https://github.com/AndiHappy/customcamunda/blob/master/src/test/java/com/zlz/customcamunda/multIInstance/CamundaMultiInstanceLoopCharacteristics.java) 
8. 自由跳转，主要的是跳转的活动的标识:[具体的实现](https://github.com/AndiHappy/customcamunda/wiki/%E8%87%AA%E7%94%B1%E8%B7%B3%E8%BD%AC)     

---

下一步主要就是专注Camunda的内部，引擎的实现以及外部的API和Model的图形界面，敬请期待     

