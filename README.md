# Java Notebook

A github repository to easily start a codespace to play with java notebooks.

## Getting started

Click on *Use this template* to create a new repository based on this one.

In *Code*, choose *Create new Codespace".

## Jupyter Kernel

This project uses [Rapaio](https://github.com/padreati/rapaio-jupyter-kernel) as Jupyter Kernel.

## Crédits
- Jules Bordais
- Rémy Curis

## Étape 1 - Introduction

import java.util.Scanner;

public class PanierAchat {
    public static void main(String[] args) {
        // Etape 3 : Déclaration des variables
        String nomProduit1 = "Stylo";
        double prixUnitaire1 = 1.20;
        int quantite1 = 5;

        String nomProduit2 = "Cahier";
        double prixUnitaire2 = 3.50;
        int quantite2 = 2;

        double total = (prixUnitaire1 * quantite1) + (prixUnitaire2 * quantite2);

## Étape 2 - Affichage d'un tableau

        System.out.println("+-----------------+--------+-------+-------+");
        System.out.println("| Produit        | PU     | Qté   | Prix  |");
        System.out.println("+-----------------+--------+-------+-------+");
        System.out.printf("| %-15s | %-6.2f | %-5d | %-6.2f |\n", nomProduit1, prixUnitaire1, quantite1, prixUnitaire1 * quantite1);
        System.out.printf("| %-15s | %-6.2f | %-5d | %-6.2f |\n", nomProduit2, prixUnitaire2, quantite2, prixUnitaire2 * quantite2);
        System.out.println("+-----------------+--------+-------+-------+");

## Étape 3 - Affichage de variables
        System.out.println("\nDétails du panier d'achat :");
        System.out.printf("Produit 1 : %s, Prix Unitaire : %.2f€, Quantité : %d, Total : %.2f€\n", nomProduit1, prixUnitaire1, quantite1, prixUnitaire1 * quantite1);
        System.out.printf("Produit 2 : %s, Prix Unitaire : %.2f€, Quantité : %d, Total : %.2f€\n", nomProduit2, prixUnitaire2, quantite2, prixUnitaire2 * quantite2);
        System.out.printf("Total du panier : %.2f€\n", total);

        // Etape 4 : Saisie des informations
        Scanner scanner = new Scanner(System.in);

        System.out.print("\nEntrez la quantité de stylos : ");
        quantite1 = scanner.nextInt();

        System.out.print("Entrez la quantité de cahiers : ");
        quantite2 = scanner.nextInt();

        // Calcul du total avec les nouvelles quantités
        total = (prixUnitaire1 * quantite1) + (prixUnitaire2 * quantite2);

        // Affichage du panier avec les quantités saisies
        System.out.println("\n+-----------------+--------+-------+-------+");
        System.out.println("| Produit        | PU     | Qté   | Prix  |");
        System.out.println("+-----------------+--------+-------+-------+");
        System.out.printf("| %-15s | %-6.2f | %-5d | %-6.2f |\n", nomProduit1, prixUnitaire1, quantite1, prixUnitaire1 * quantite1);
        System.out.printf("| %-15s | %-6.2f | %-5d | %-6.2f |\n", nomProduit2, prixUnitaire2, quantite2, prixUnitaire2 * quantite2);
        System.out.println("+-----------------+--------+-------+-------+");

        // Affichage du total
        System.out.printf("\nTotal du panier : %.2f€\n", total);
    }
}
