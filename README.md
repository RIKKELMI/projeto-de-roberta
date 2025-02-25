# projeto-de-roberta
package projetoaula;
import java.util.Scanner;
public class qaafaefaeadeaaea {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
	        Scanner s = new Scanner(System.in);

	        while (true) {
	            System.out.println("Você é professor? Digite 1 para Sim e 2 para Não.");
	            int professor = s.nextInt();
	            s.nextLine(); 

	            if (professor == 2) {
	                System.out.println("Tudo bem, você vai sair do nosso programa, pois somente professores podem ter acesso ao Mapa de Ensino.");
	                System.out.println("Reiniciando o programa...");
	                continue; 
	            } else if (professor == 1) {
	                System.out.println("Qual sua disciplina?");
	                System.out.println("Digite 1 para Informática, 2 para Geografia, 3 para Biologia, 4 para Química.");
	                int disciplina = s.nextInt();
	                s.nextLine();

	                System.out.println("Digite 1 para Aula Teórica e digite 2 para Aula Prática.");
	                int tipoAula = s.nextInt();
	                s.nextLine();

	                if (disciplina == 1) { 
	                    if (tipoAula == 1) {
	                        System.out.println("Aula teórica será realizada na sala de aula.");
	                    } else if (tipoAula == 2) {
	                        System.out.println("Aula prática de programação realizada no laboratório de informática 1.");
	                    }
	                } else if (disciplina == 2) { 
	                    if (tipoAula == 1) {
	                        System.out.println("Aula teórica será realizada na sala de aula.");
	                    } else if (tipoAula == 2) {
	                        System.out.println("Sugestão: Utilizar ferramentas de gamificação para tornar a aula mais interativa.");
	                    }
	                } else if (disciplina == 3) { 
	                    if (tipoAula == 1) {
	                        System.out.println("Aula teórica será realizada na sala de aula.");
	                    } else if (tipoAula == 2) {
	                        System.out.println("Aula prática realizada no laboratório de informática 3. Professor(a) deve realizar atividade de busca sobre Mitocôndrias.");
	                    }
	                } else if (disciplina == 4) { 
	                    if (tipoAula == 1) {
	                        System.out.println("Aula teórica será realizada na sala de aula.");
	                    } else if (tipoAula == 2) {
	                        System.out.println("Aula prática realizada no laboratório de química. Tenha cuidado ao manusear os produtos químicos.");
	                    }
	                }

	                System.out.println("Se deseja sair, digite 'sair'. Caso contrário, o programa reiniciará.");
	                String sair = s.nextLine();
	                if (sair.equalsIgnoreCase("sair")) {
	                    System.out.println("Tudo bem! Até a próxima! O Mapa de Ensino agradece.");
	                    break;
	                }
	            }
	        }

	        s.close();
	    }
	}
