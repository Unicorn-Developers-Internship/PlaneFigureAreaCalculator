package com.UnicornDevelopers;


import java.util.InputMismatchException;
import java.util.Scanner;

public class planeShapeAreaCalculator {
    public static void main(String[] arg) {
        displayListOfShapes();
        int figureOption = figureOption();
        System.out.println("Assuming all measurements are in meters(m)");
        //calculate an area based on figure chosen
        switch (figureOption) {
            case 1 -> triangleArea();
            case 2 -> squareArea();
            case 3 -> parallelogramArea();
            case 4 -> rectangleArea();
            case 5 -> trapeziumArea();
            case 6 -> circleArea();
            default -> System.out.println("No area calculated!");
        }



    }

    //plane figure options method
    public static void displayListOfShapes() {
        System.out.println("*************************************************************");
        System.out.println("Hi! Welcome to figureGenius!\nThis app helps you to easily calculate the area of common plane figures.");
        System.out.println("**************************************************************");
        System.out.println("Below is a list of plane Shapes you can choose from.");
        System.out.println("Select the type of plane figure you want to calculate it's area by providing it's option number\n(e.g Enter 1 to choose Triangle, 2 to choose Square,...)\n");
        System.out.println("""
                ************************************************************
                1.TRIANGLE                                                 *
                2.SQUARE                                                   *
                3.PARALLELOGRAM                                            *
                4.RECTANGLE                                                *
                5.TRAPEZIUM OR TRAPEZOID                                   *
                6.CIRCLE                                                   *
                ************************************************************
                """);


    }
    //choose figure option method
    public static int figureOption(){
        Scanner optionInput = new Scanner(System.in);
        int figureOptionNumber = 0;
        System.out.println("Enter an option number to choose the figure you want to find it's AREA\n" +
                "(Enter 1 or 2 or 3 or 4 or 5 or 6 to choose a figure):");
        try {
            figureOptionNumber = optionInput.nextInt();
            if (figureOptionNumber <= 0 || figureOptionNumber >6 ){
                throw new Exception();
            }
        }catch (InputMismatchException e){
            System.out.println("Wrong input. Enter any option only form 1 to 6.");
        }catch (Exception e){
            System.out.println("Number is not available in the options 1 to 6.");
        }

        return figureOptionNumber;

    }

    //Triangle area method
    public static void triangleArea(){
        System.out.println("\nShort Description:\nTRIANGLE: A triangle is a plane figure with three(3) sides and three(3) angles");
        System.out.println("\tTo calculate the area of a triangle, you need the Height(H) and Base(B) of the triangle.\n" +
                "Formula for Area: Area = 1/2(Base * Height)");
        double height,base; //height and base of triangle
        Scanner input = new Scanner(System.in);
        System.out.println("Enter the Height(H):");
        height = input.nextDouble();
        System.out.println("Enter the Base(B):");
        base = input.nextDouble();
        double triangleArea = 0.5*(base*height);
        System.out.printf("The AREA of your triangle which has Height %.2fm and Base %.2fm is %.2f meterSquared\n",height,base,triangleArea);
    }

    //method to find area of Square
    public static void squareArea(){
        System.out.println("\nShort Description:\nSQUARE: A square is a plane figure with four(4) sides of equal length");
        System.out.println("\tTo calculate the area of a square, you need only one of the length of it's sides.\n" +
                "Formula for Area: Area = L * L (L squared)");
        double length; //length of a side of the square
        Scanner input = new Scanner(System.in);
        System.out.println("Enter a length of any sides of the square:");
        length = input.nextDouble();
        double squareArea = length * length;
        System.out.printf("The AREA of your square which has length %.2fm is %.2f meterSquared\n",length,squareArea);
   }

   //Parallelogram area method
    public static void parallelogramArea(){
        System.out.println("""
                Short Description:
                PARALLELOGRAM: A parallelogram is a quadrilateral with opposite sides parallel
                and therefore opposite angles equal.""");
        System.out.println("\tTo calculate the area of a parallelogram, you need the Height(H) and Base(B) of the parallelogram.\n" +
                "Formula for Area: Area = Base * Height");
        double height,base; //height and base of triangle
        Scanner input = new Scanner(System.in);
        System.out.println("Enter the Base(H):");
        base = input.nextDouble();
        System.out.println("Enter the Height(H):");
        height = input.nextDouble();
        double parallelogramArea = base * height;
        System.out.printf("The AREA of your parallelogram which has base %.2fm and height %.2fm is %.2f meterSquared",base,height,parallelogramArea);
    }

    //Rectangle area method
    public static void rectangleArea() {
        System.out.println("\nShort Description:\nRECTANGLE: A rectangle is a plane figure with four(4) right angles and four sides.");
        System.out.println("\tTo calculate the area of a rectangle, you need the Breath(B) or Width(W) and the Length(L) of the rectangle .\n" +
                "Formula for Area: Area = L * W ");
        double width, length;
        Scanner input = new Scanner(System.in);
        System.out.println("Enter the width(W):");
        width = input.nextDouble();
        System.out.println("Enter the length(L):");
        length = input.nextDouble();
        double rectangleArea = length * width;
        System.out.printf("The AREA of your triangle which has width %.2fm and length %.2fm is %.2f meterSquared.", width, length, rectangleArea);
    }

    //Trapezium area method
    public static void trapeziumArea(){
        System.out.println("\nShort Description:\nTRAPEZIUM or TRAPEZOID: A trapezium is a quadrilateral with no parallel sides.");
        System.out.println("\tTo calculate the area of a trapezium, you need the vertical Height(H) and the sum of the length of top(a) and the length of base(b).\n" +
                "Formula for Area: Area = 1/2 H(a + b)");
        double height, top, base;//height,top and base length of trapezium
        Scanner input = new Scanner(System.in);
        System.out.print("Enter height(H):");
        height = input.nextDouble();
        System.out.print("\tEnter top length(a):");
        top = input.nextDouble();
        System.out.print("\tEnter base length(b):");
        base = input.nextDouble();
        double trapeziumArea = 0.5*height*(top + base);
        System.out.printf("The AREA of your trapezium which has height(H) of %.2fm, top length(a) of %.2fm\nand a base length(b) of %.2fm is %.2f meterSquared. ", height,top,base,trapeziumArea);
    }

    //Circle area method
    public static void circleArea(){
        System.out.println("\nShort Description:\nCIRCLE: A circle is a round shaped figure that has no corners or edges.");
        System.out.println("\tTo calculate the area of a circle, you need the radius(r) of the circle.\n" +
                "Formula for Area: Area = ∏*r*r");
        double radius;//radius of circle
        Scanner input = new Scanner(System.in);
        System.out.println("Enter radius(r) of circle:");
        radius = input.nextDouble();
        double circleArea = Math.PI*radius*radius;
        System.out.printf("The AREA of your circle with radius(r) of %.2fm is %.2f meterSquared.\n",radius, circleArea);
    }
    }


