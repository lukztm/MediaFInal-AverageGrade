# MediaFinal-AverageGrade
Recebe duas notas, mostra a media final do aluno e diz se ele foi reprovado, se está de recuperação ou se foi reprovado. 

	public static void main(String[] args) {

		Double nota1 = 0.0;
		Double nota2 = 0.0;
		int contadornota = 1;

		while (contadornota == 1) {
			String entrada = JOptionPane.showInputDialog("Digite a nota do aluno:");
			entrada = entrada.replace(',', '.');
			nota1 = Double.parseDouble(entrada);
			System.out.println("A primeira nota foi: " + nota1);
			contadornota++;
		}
		if (contadornota == 2) {
			String entrada = JOptionPane.showInputDialog("Digite a nota do aluno:");
			entrada = entrada.replace(',', '.');
			nota2 = Double.parseDouble(entrada);
			System.out.println("A segunda nota foi: " + nota2);
			contadornota++;

			Double media = ((nota1 + nota2) / 2);
			System.out.println("Sua media final foi: " + media);

			if (media >= 7 && media <= 10) {
				System.out.println("Aluno aprovado!!!");
			}
			if (media >= 4 && media < 7) {
				System.out.println("Aluno em recuperação!!");
			}
			if (media >= 0 && media < 4) {
				System.out.println("Aluno reprovado!");
			}
			if (media < 0 || media > 10) {
				System.out.println("Digite valores válidos.");
			}
		}
	}
}

!!!ENGLISH!!!
Gets two grades and shows the average grade.

	public static void main(String[] args) {

		Double grade1 = 0.0;
		Double grade2 = 0.0;
		int countergrade = 1;

		while (countergrade == 1) {
			String in = JOptionPane.showInputDialog("Type the grade:");
			in = in.replace(',', '.');
			note1 = Double.parseDouble(in);
			System.out.println("The first grade was: " + grade1);
			countergrade++;
		}
		if (countergrade == 2) {
			String in = JOptionPane.showInputDialog("Type the grade:");
			in = in.replace(',', '.');
			grade2 = Double.parseDouble(in);
			System.out.println("The secound grade was: " + grade2);
			countergrade++;

			Double average = ((grade1 + grade2) / 2);
			System.out.println("Your average grade is: " + average);

			if (average >= 7 && average <= 10) {
				System.out.println("Congratulations!!!");
			}
			if (average >= 4 && average < 7) {
				System.out.println("You need to study harder!!");
			}
			if (average >= 0 && average < 4) {
				System.out.println("Bad grade!");
			}
			if (average < 0 || average > 10) {
				System.out.println("Type valid values.");
			}
		}
	}
}
