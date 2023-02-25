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
