# LogginString
Loggin String con 3 intentos
package clasesiete;

import java.util.Scanner;

public class ejercicioUnoOpcionString {
	
	public static void main(String[] args) {
		
		Scanner entrada = new Scanner(System.in);
		int intentos = 0;
		int resto = 3;
		String name;
		
		do {
			System.out.println("Ingrese su password por favor");
			name = entrada.next();
			
			if (name.equalsIgnoreCase("Lucia")) {System.out.println("¡Bienvenido usuario!");
			intentos = 3;}
			
			else {System.out.println("Contraseña incorrecto, usted tiene " + (--resto) + " intentos");
			intentos = intentos + 1;
			
			if (intentos == 3) System.out.println("Acceso reestringido, comuniquese con el administrador");
			}
			
		}while (intentos < 3);
		
	}

}
