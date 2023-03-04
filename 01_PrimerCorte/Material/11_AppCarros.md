## App Carros

### AppCars.java
```Java
package appcars;

public class AppCars {   
    public static void main(String[] args) {
       System.out.println("App de Carreras de Carros");
       
       Car car1=new Car("2023","Mazada","negro");
       Car car2=new Car("2022","Susuki","gris");
       Car car3=new Car("2022","Mercedez","rojo");
       
       mostrarInfo(car1);       
       generarVelocidad(car1);
       System.out.println("Velocidad : "+car1.getVelocidad());
          
       
       System.out.println("");       
       mostrarInfo(car2);
       generarVelocidad(car2);
       System.out.println("Velocidad : "+car2.getVelocidad());
       
       System.out.println("");       
       mostrarInfo(car3);
       generarVelocidad(car3);
       System.out.println("Velocidad : "+car3.getVelocidad());
      
              
    }
    
    public static void mostrarInfo(Car carro){
       System.out.println("Modelo: "+carro.getModelo());
       System.out.println("Marca : "+carro.getMarca());
       System.out.println("Color : "+carro.getColor());
       System.out.println("Motor encedido : "+carro.isEncendidoMotor());
       System.out.println("Velocidad : "+carro.getVelocidad());
    }
    public static void generarVelocidad(Car car){
       for(int i=0;i<5;i++){
          car.acelerar((int)Math.floor(Math.random()*50+1));    
       }
       
    
    }
    
    
    
}
```

### Cars.java
```Java
package appcars;

public class Car {
    
    //Atributos
    private String modelo;
    private String marca;
    private String color;
    private int    velocidad;
    private boolean encendidoMotor;
    
    //Métodos
    public void Car(){}

    public Car(String modelo, String marca, String color) {
        this.modelo = modelo;
        this.marca = marca;
        this.color = color;
        this.encendidoMotor=false;
        this.velocidad=0;
    }

    public String getModelo() {
        return modelo;
    }

    public void setModelo(String modelo) {
        this.modelo = modelo;
    }

    public String getMarca() {
        return marca;
    }

    public void setMarca(String marca) {
        this.marca = marca;
    }

    public String getColor() {
        return color;
    }

    public void setColor(String color) {
        this.color = color;
    }

    public int getVelocidad() {
        return velocidad;
    }

    public void setVelocidad(int velocidad) {
        this.velocidad = velocidad;
    }

    public boolean isEncendidoMotor() {
        return encendidoMotor;
    }

    public void setEncendidoMotor(boolean encendidoMotor) {
        this.encendidoMotor = encendidoMotor;
    }
    
    public void encenderMotor(){      
        if(this.encendidoMotor==true){
           System.out.println("Pilas ya estoy encendido");
        }else{
           this.encendidoMotor=true;
           System.out.println("Runnnnnnnn!!!");
        }    
    }
    
    public void acelerar(int acelerada){
      this.velocidad=this.velocidad+acelerada;
    }
    
    public void frenar(int frenada){
       if(this.velocidad-frenada>0){
          this.velocidad=this.velocidad-frenada;
       }else{
         this.velocidad=0;
         System.out.println("Ya estoy detenido en velociada 0");
       }
    }
    
    
    
}
```
