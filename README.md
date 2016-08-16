# js-get-sibling
js获取兄弟节点兼容方法
    
    //获取上一个兄弟节点
    function getPreviousSibling(n){
      var x=n.previousSibling;
      while(x.nodeType!=1){
        x=x.previousSibling;
      }
      return x;
    }
    //获取下一个兄弟节点
    function getNextSibling(n){ //传入需要访问的节点
      var x=n.nextSibling;
      while(x.nodeType!=1){
        x=x.nextSibling;
      }
      return x;
    }
    
