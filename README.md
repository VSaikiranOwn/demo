demo
====

Logical Programs
package com;

import java.math.BigDecimal;

public class FloatingPoints {

	private double number1 = 10.45;
	private double number2 = 9.30;

	private BigDecimal decNum1 = new BigDecimal(10.45);
	private BigDecimal decNum2 = new BigDecimal(9.30);

	private BigDecimal decimalNum1 = new BigDecimal("10.45");
	private BigDecimal decimalNum2 = new BigDecimal("9.30");

	public void subtractDoubleValues() {
		System.out.println("Subtraction With Double Data Types : " + (number1 - number2));
		System.out.println("Subtraction With Double Constructor of Big Decimal Class : " + (decNum1.subtract(decNum2)));
		System.out.println("Subtraction With String Constructor of Big Decimal Class : " + (decimalNum1.subtract(decimalNum2)));
	}
	public static void main(String[] args) {

		FloatingPoints floatingPoint = new FloatingPoints();
		floatingPoint.subtractDoubleValues();

	}
}
