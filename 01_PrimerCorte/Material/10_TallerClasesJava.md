# Taller de Clases en Java


## 1. Viajero.java

```Java
package guerrocamino;

public class Viajero {

    //Atributos
    public String nombres;

    public String apellidos;

    public String celular;

    public String direccion;

    public String fechaNacimiento;

    //Métodos
    
    public Viajero(){
    
    }

    public Viajero(String nombres, String apellidos, String celular, String direccion, String fechaNacimiento) {
        this.nombres = nombres;
        this.apellidos = apellidos;
        this.celular = celular;
        this.direccion = direccion;
        this.fechaNacimiento = fechaNacimiento;
    }

    public String getNombres() {
        return nombres;
    }

    public void setNombres(String nombres) {
        this.nombres = nombres;
    }

    public String getApellidos() {
        return apellidos;
    }

    public void setApellidos(String apellidos) {
        this.apellidos = apellidos;
    }

    public String getCelular() {
        return celular;
    }

    public void setCelular(String celular) {
        this.celular = celular;
    }

    public String getDireccion() {
        return direccion;
    }

    public void setDireccion(String direccion) {
        this.direccion = direccion;
    }

    public String getFechaNacimiento() {
        return fechaNacimiento;
    }

    public void setFechaNacimiento(String fechaNacimiento) {
        this.fechaNacimiento = fechaNacimiento;
    }
        
    
}

```
## 2. GuerreroCamino.java

```Java
package guerrocamino;

public class GuerroCamino {
    
    public static void main(String[] args) {
        
        System.out.println("Inicio App Guerrero del Camino");
        
        Viajero viajero1=new Viajero("Camilo Ernesto","Rodriguez Moreno","30045686","Cra 28 #45-3","1994/09/03");
        Viajero viajero2=new Viajero("Diego Fernando","Rangel Perez","30045686","Cra 109 #45-3","200/05/15");
        
        System.out.println("Datos de los viajeros");        
        System.out.println("Viajero1:");
        System.out.println("Nombres:"+viajero1.getNombres());
        System.out.println("Apellidos:"+viajero1.getApellidos());
        System.out.println("Viajero2:");
        System.out.println("Nombres:"+viajero2.getNombres());
        System.out.println("Apellidos:"+viajero2.getApellidos());
    }
}

```
