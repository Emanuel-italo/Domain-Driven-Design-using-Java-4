# Domain-Driven-Design-using-Java-4
Treinamento itensivo - Java


//Escreva um programa que leia as medidas dos lados de um triângulo e escreva se ele é Equilátero, Isósceles ou Escaleno.
// Sendo que:
// − Triângulo Equilátero: possui os 3 lados iguais. − Triângulo Isóscele: possui 2 lados iguais.
// − Triângulo Escaleno: possui 3 lados diferentes.

import java.util.Scanner;

public class IntensivoJava4 {
public static void main(String[] args) {
Scanner scanner = new Scanner(System.in);

        System.out.println("Digite o primeiro lado do triângulo: ");
        float primeiro = scanner.nextFloat();

        System.out.println("Digite o segundo lado do triângulo: ");
        float segundo = scanner.nextFloat();

        System.out.println("Digite o terceiro lado do triângulo: ");
        float terceiro = scanner.nextFloat();


        if (primeiro == segundo && segundo == terceiro) {
            System.out.println("O triângulo é Equilátero");
        } else if (primeiro == segundo || primeiro == terceiro || segundo == terceiro) {
            System.out.println("O triângulo é Isósceles");
        } else {
            System.out.println("O triângulo é Escaleno");
        }

        scanner.close();
    }
}
