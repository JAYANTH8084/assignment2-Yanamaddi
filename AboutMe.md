# yanamaddi jayanth 
My self jayanth yanamaddi done my graduation in year 2018. I worked as an SAP abap developer in TechM, India. I love to ride KTM bikes. I frequently go on KTM organised trips.<br> I have an experience of 2 years in Techm. Looking forward for a great career in united states.


![ My Image](/jayanth.jpg?raw=true)

# Food and Drinks
The below table describes the Food and Drinks available at the best deals in the nearby locations.

| Food/Drink |   Place     |  Price  |
| ---------- |   -----     |  ------ |
|  Pepsi     |    MCD      |   2$    |
|  Fries     |    KFC      |   5$    |
|  Noodles   |    Tachos   |   3$    |
|  Nuggets   |    B King   |   7$    |

---

# Pithy Quotes

> The greatest glory in living lies not in never falling, but in rising every time we fall. -*Nelson Mandela*

> Your time is limited, so don't waste it living someone else's life. Don't be trapped by dogma – which is living with the results of other people's thinking. -*Steve Jobs*

---

# Algebra algorithm
> Algebra is one of the definitive and oldest branches of mathematics, and design of computer algorithms is one of the youngest. Despite this generation gap, the two disciplines beautifully interweave. Firstly, modern computers would be somewhat useless if they were not able to carry out arithmetic and algebraic computations efficiently, so we need to think on dedicated, sometimes rather sophisticated algorithms for these operations. Secondly, algebraic structures and theorems can help develop algorithms for things having [at first glance] nothing to do with algebra, e.g. graph algorithms. One of the main goals of the offered course is thus providing the learners with the examples of the above mentioned situations. We believe the course to contain much material of interest to both CS and Math oriented students. The course is supported by programming assignments.
[Source]( https://www.coursera.org/learn/algebra-and-algorithms)

```
int gcd(int a, int b, int& x, int& y) {
    if (b == 0) {
        x = 1;
        y = 0;
        return a;
    }
    int x1, y1;
    int d = gcd(b, a % b, x1, y1);
    x = y1;
    y = x1 - y1 * (a / b);
    return d;
}

bool find_any_solution(int a, int b, int c, int &x0, int &y0, int &g) {
    g = gcd(abs(a), abs(b), x0, y0);
    if (c % g) {
        return false;
    }

    x0 *= c / g;
    y0 *= c / g;
    if (a < 0) x0 = -x0;
    if (b < 0) y0 = -y0;
    return true;
}
```
[Source](https://cp-algorithms.com/algebra/linear-diophantine-equation.html)