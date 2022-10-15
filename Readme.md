Q1 https://github.com/rvsp/typescript-oops/blob/master/Practice/Movie.md
Ans.
 class Movie{
      constructor(title,studio,rating="PG"){
            this.title=title;
            this.studio=studio;
            this.rating=rating;  
         }
         getPG(movie){
            for(var i in movie){
                if(movie[i].rating==="PG"){
                    arr.push(movie[i].title);
                      }     
                               }
            return arr;
          }
       }
   const arr=[];
   var movie=[{title:"123",studio:"south",rating:"P"},{title:"1234",studio:"north",rating:"PG"},{title:"12345",studio:"west",rating:"PG"}]
   let movie1=new Movie(movie)
   console.log("Movies where rating=PG  "+movie1.getPG(movie))
   var movie2=new Movie("Casino Royale","Eon Productions","PG13")
   console.log("Title of movie is----->"+movie2.title+"Studio of movie is----->"+ movie2.studio+"Rating of movie is------>"+ movie2.rating)
 
 
 Q2 https://github.com/rvsp/typescript-oops/blob/master/Practice/class-circle.md
   Ans.
    public class Circle{
      private Number radius;
      private String color;
        }
       public Circle()
       public Circle(Number radius)
       public Circle(Number radius,String color )
       public Number getRadius()
       {
        return radius;
       }
       public void setRadius(Number radius)
       public String getColor()
      {
        return colour;
      }
       public void setColor(String color)
       public String toString()
       public Number getArea()
      {
        return (3.14*radius*radius);
      }
       public Number getCircumference()
      {
        return (2*3.14*radius);
      }
      
  Q3 Write a “person” class to hold all the details
  Ans. 
  class Person{
    constructor(name,age,qualification,job,country)
      {
        this.name=name;
        this.age=age;
        this.qualification=qualification;
        this.job=job;
        this.country=country;
        this.fulldetails = function(){
            return [this.name+"  "+this.age+"  "+this.qualification+"  "+this.job+"  "+this.country];
          }
      }
       }
      let person=new Person ( "Manoj","25","Graduate","Quality-manager","India" )
      console.log(person.fulldetails());
      
 Q4 Write a class to calculate the uber price
 Ans.
 class Uber{
               constructor(price,kilometer){
                    this.price=price
                    this.kilometer=kilometer
                    }
                  calculate(price,kilometer){
                        return price*kilometer
                      }
      }
var totalprice=new Uber(100,7)
console.log(totalprice.calculate(100,7))

