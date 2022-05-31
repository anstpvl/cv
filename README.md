# Anastasiya Pavlovskaya
### Future HR manager

### Contact information:
##### **Phone:** +375(33)337-25-42 
##### **Email:** pavlovskya2003@gmail.com
##### **Inst:** anst_pvl
##### **Tg:** Paastyaa

### Soft skills:
- Responsibility
- High communication skills
- Time managment skills
- Flexibility
- Critical thinking

### Skills:
- Adobe Photoshop, Canva
- C++
- Microsoft Word/Excel
- Git, Github
- English level - B2
- Cmd, Linux

### Code:
```c++
class cube {
protected:
    int a;
public:
    cube(int a) {
        this->a = a; 
    }
    int get_a() {
        return a;
    }
    int volume() {
        return a * a * a;
    }
};

class parallelepiped : public cube {
protected:
    int a, b, c;
public:
    parallelepiped(int a, int b, int c) :cube(a) {
        this->a = a;
        this->b = b;
        this->c = c;
    }
    int get_a() {
        return a;
    }
    int get_b() {
        return b;
    }
    int get_c() {
        return c;
    }
    int volume() {
        return a * b * c;
    }
};

int main() {

    setlocale(0, "rus");
    int x, y, z;
    cout << "введите 3 числа через пробел для задания параметров фигур: ";
    cin >> x >> y >> z;

    if (x <= 0 && y <= 0 && z <= 0) {
        cout << "ERROR!\n";
        exit(-1);
    }

    cube rec(x); //вызов конструктора для куба
    cout << "V_куба = " << rec.volume() << "\n";

    parallelepiped trap(x, y, z); //вызов конструктора для параллелепипеда
    cout << "V_параллелепипеда = " << trap.volume() << "\n";
    system("pause");
    return 0;
}
