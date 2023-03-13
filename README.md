## 2023 C++프로그래밍
---------------------
---------------------

생성자는 return값이 없다.
생성자는 초기화를 위해 사용 (클래스 이름과 같아야함)
생성자는 오버로딩 할 수 있음

중복정의 : 같은 이름인데 매개변수가 다르다.
<CRect라는 클래스는 4각형을 처리 하기 적합하다. 
두 개의 멤버변수 w, h를 가지며, 면적을 구해서 리턴하는 Area()함수를 가진다.
초기값으로 4와5로 초기화를 할 수도 있고, 내가 생성자에 값을 넣을 수도 있다. 
면적을 C++기반 클래스로 코딩하고 포인터로 출력하는 코드를 작성하시오.>
#include <iostream>
using namespace std;
class CRect{
    int w, h;
    public:
    CRect(){ w=4; h=5;}
    CRect(){int a, int b}{
        w= a; h=b;
    }
    int Area(){ return w*h;}
};
int main(){
    CRect r(20,30);
    CRect* p;
    p=&r;
    cout << p->Area()
    return 0;
}
----------------------
//사각형 면적 구하는 class CRect 활용해 {4,5}면적 구하는 C++코드작성//
#include <iostream>
using namespace std;

class CRect{
    int w,h;
    public:
        CRect(){w=2, h=3;}
        int Area(){return w*h;}
};

class CTri{
    int w,h;
    public:
        CTri(){w=2, h=3;}
        int Area(){return (w*h/2);}
};
int main(){
    CRect r;
    CTri t;
    cout<<r.Area()<<" "<<t.Area();

    return 0;
}



