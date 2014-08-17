//  Created by Carlos Andres Vargas Farfan on 2014-08-16.
//  Copyright (c) 2014 Carlos Vargas. All rights reserved.
//

import UIKit

class Node: NSObject{
    internal var data: AnyObject?
    internal var next: Node?
    
    override init(){
        
        data =  nil
        next =  nil
    }
}


class Stack: NSObject {
    
    var head: Node?
    var count: Int
    
    override init()
    {
        head = nil
        count = 0
    }
    
    func push(aData: AnyObject){
        
        var newHead =  Node()
        newHead.data = aData
        
        if(head == nil){
            newHead.next = nil
            head = newHead
        }
        else{
            newHead.next = head
            head =  newHead
        }
        
        count++
    }
    
    func pop() -> AnyObject?{
        
        if(count == 0){
            return nil
        }
        else{
            var dataNode = head
            head =  dataNode?.next
            dataNode?.next = nil
            count--
            return dataNode?.data
        }
    }
    
    func size() -> Int{
        return count
    }
}
