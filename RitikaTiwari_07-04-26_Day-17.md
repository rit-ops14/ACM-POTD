#Day 17- (implement stack using queues)

##Date - 07/04/26

##Problem - implement stack using queues


##code(C++)- '''class MyStack {
private:
    queue<int> q;
    
public:
    MyStack() {}
    
    void push(int x) {
        q.push(x);
        for (int i = 1; i < q.size(); i++) {
            q.push(q.front());
            q.pop();
        }
    }
    
    int pop() {
        int res = q.front();
        q.pop();
        return res;
    }
    
    int top() {
        return q.front();
    }
    
    bool empty() {
        return q.empty();
    }
  };  '''
