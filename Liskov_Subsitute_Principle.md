# Liskov Substitution Prensibi

## Liskov Substitution Presibinin Amacı Nedir?,
- Kodlarımızda herhangi bir değişiklik yapmaya gerek duymadan alt sınıfları, türedikleri(üst) sınıfların yerine kullanabilmeliyiz.
- Liskov Substitution Prensibi, bir sınıfın başka bir sınıfa kalıtımının kontrolünü sağlamaktır.

## Liskov Substitution Prensibi Nedir?

- Liskov Substitution Prensibi, herhangi bir sınıfın başka bir sınıfa kalıtım yapılmasının, sınıfın özelliklerini değiştirmeyeceğini belirtir.
- Liskov Substitution Prensibi, her türlü nesne için, kalıtım yapısının kullanılmasını sağlar.

## Liskov Substitution Prensibi Nasıl Çalışır?

java code example for Lsp :

    public class Rectangle {

        public int width;
        public int height;

        public Rectangle(int width, int height) {
            this.width = width;
            this.height = height;
        }

        public int getArea() {
            return width * height;
        }
    }

    public class Square extends Rectangle {

        public Square(int side) {
            super(side, side);
        }
    }

    public class Test {
        public static void main(String[] args) {
            Rectangle rectangle = new Rectangle(10, 20);
            System.out.println(rectangle.getArea());

            Square square = new Square(10);
            System.out.println(square.getArea());
        }
    }

- Rectangle sınıfı,Square sınıfı tarafından extend edildi ve getArea() metodu override edildi.
- Square sınıfı,Rectangle sınıfının getArea() metodunu override etmek istemediğimizden, Liskov Substitution Prensibi kullanıldı.
- Türeyen sınıf yani alt sınıflar ana(üst) sınıfın tüm özelliklerini ve metotlarını aynı işlevi gösterecek şekilde kullanabilme ve kendine ait yeni özellikler barındırabilmelidir. Ana amacımız bu.
