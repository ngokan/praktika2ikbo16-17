# praktika2ikbo16-17
Нгуен Куок Ань ИКБО-16-17

Main.java


package com.company;

public class Main {

    public static void main(String[] args) {

        System.out.println("exercise 1");
        //exercise 1
        Ball b1, b2, b3;
        b1 = new Ball();
        b2 = new Ball("green");
        b3 = new Ball("blue",5);

        b1.setColor("red");
        b1.setRadius(3);

        b1.getColor();
        b1.getRadius();

        System.out.println(b1);

        System.out.println("exercise 2");
        //exercise 2
        Book book1, book2, book3;
        book1 = new Book();
        book2 = new Book("The great adventure");
        book3 = new Book("From the hell","Ethan");

        book1.setName("The broken heart");
        book1.setAuthor("Jackson");

        book1.getName();
        book1.getAuthor();

        System.out.println(book1);
    }
}
------------------------------------------------------
Ball.java


package com.company;
import java.lang.*;

public class Ball {
    private String color;
    private int radius;

    public Ball(){
        this.color = "unknown";
        this.radius = 0;
    }
    public Ball(String c){
        this.color = c;
        this.radius = 0;
    }
    public Ball(String c, int r) {
        this.color = c;
        this.radius = r;
    }

    public void setColor(String c){
        this.color = c;
    }
    public void setRadius(int r){
        this.radius = r;
    }

    public String getColor(){
        return this.color;
    }
    public int getRadius(){
        return this.radius;
    }

    public String toString(){
        return "The color of the ball is " + this.color + ". The radius of this ball is " + this.radius + '.';
    }
}
------------------------------------------------------
Book.java


package com.company;
import java.lang.*;

public class Book {
    private String name;
    private String author;

    public Book(){
        this.name = "unknown";
        this.author = "unknown";
    }
    public Book(String n){
        this.name = n;
        this.author = "unknown";
    }
    public Book(String n, String a) {
        this.name = n;
        this.author = a;
    }

    public void setName(String n){
        this.name = n;
    }
    public void setAuthor(String a){
        this.author = a;
    }

    public String getName(){
        return this.name;
    }
    public String getAuthor(){
        return this.author;
    }

    public String toString(){
        return "The  name of the book is " + this.name + ". The name of the author is " + this.author + '.';
    }
}

