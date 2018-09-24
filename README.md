# praktika2ikbo16-17
Нгуен Куок Ань ИКБО-16-17

Author.java


package com.company;
import java.lang.*;

public class Author {

    private String name;
    private String email;
    private char gender;

    public Author(String n,String e,char g){
        this.name = n;
        this.email = e;
        this.gender = g;
    }

    public void setEmail(String e){
        this.email = e;
    }
    public String getName(){
        return this.name;
    }
    public String getEmail(){
        return this.email;
    }
    public char getGender(){
        return this.gender;
    }

    public String toString(){
        return this.name + '(' + this.gender + ") at " + this.email;
    }

}
-----------------------------------
Main.java


package com.company;

public class Main {

    public static void main(String[] args) {
	    Author a = new Author("Nguyen Quoc Anh","cuti_mos@mail.ru",'m');
	    a.getName();
	    a.getEmail();
	    a.getGender();
	    System.out.println(a);

        System.out.println("after set");

        a.setEmail("NguyenQ@mail.ru");
        a.getEmail();
        System.out.println(a);

    }
}


