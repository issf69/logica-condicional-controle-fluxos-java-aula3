# logica-condicional-controle-fluxos-java-aula3
Controle de Fluxo
package dio.com.br;

/**
 * Classe de exemplo para o exercicio  da Aula 3 de Operadores lógicos e relacionais, controle de fluxo e Blocos.
 */
public class Main {

    public static void main(String[] args) {

        ifFlecha();
        ifSemFlecha();
        ifFerias();
        ifMenor();

        switchSemana();
        switchNumero();
        switchFerias();
    }

    private static void ifFlecha() {

        int mes = 9;
        if (mes == 1) {
            System.out.println("Janeiro");
        } else {
            if (mes == 2) {
                System.out.println("Fevereiro");
            } else {
                if (mes == 3) {
                    System.out.println("Março");
                } else {
                    if (mes == 4) {
                        System.out.println("Abril");
                    } else {
                        if (mes == 5) {
                            System.out.println("Maio");
                        } else {
                            if (mes == 6) {
                                System.out.println("Junho");
                            } else {
                                if (mes == 7) {
                                    System.out.println("Junho");
                                } else {
                                    if (mes == 8) {
                                        System.out.println("Agosto");
                                    } else {
                                        if (mes == 9) {
                                            System.out.println("Setembro");
                                        } else {
                                            if (mes == 10) {
                                                System.out.println("Outubro");
                                            } else {
                                                if (mes == 11) {
                                                    System.out.println("Novembro");
                                                } else {
//                                                    if (mes ==12) {
                                                    System.out.println("Dezembro");
//                                                    }
//                                                   } else {
//                                                        System.out.println("Mes indefinido");
//                                                }
                                            }
                                        }
                                    }
                                }
                            }
                        }
                    }
                }
            }
        }
    }
}

    private static void ifSemFlecha () {

    int mes = 9;
    if (mes == 1) {
        System.out.println("Janeiro");
    } else if (mes == 2) {
        System.out.println("Fevereiro");
    } else if (mes == 3) {
        System.out.println("Março");
    } else if (mes ==4) {
        System.out.println("Abril");
    } else if (mes == 5) {
        System.out.println("Maio");
    } else if (mes == 6) {
        System.out.println("Junho");
    } else if (mes == 7) {
        System.out.println("Julho");
    } else if (mes == 8) {
        System.out.println("Agosto");
    } else if (mes == 9) {
        System.out.println("Setembro");
    } else if (mes == 10) {
        System.out.println("Outubro");
    } else if (mes == 11) {
        System.out.println("Novembro");
    } else {
        System.out.println("Dezembro");
    }
//    } else if (mes == 12)
//        System.out.println("Dezembro");
//    } else {
//        System.out.println("Mes indefinido");
//
//    }
}

    private static void ifFerias() {

        String mes = "julho";
        if (mes =="julho" || mes == "dezembro" || mes == "janeiro") {
            System.out.println("Ferias");
        }
    }

    private static void ifMenor() {

    double salarioMensal = 11893.58d;
    double mediaSalario = 10500d;

    int quantidadeDependentes = 4;
    int mediaDependentes = 2;

    if (salarioMensal < mediaSalario && (quantidadeDependentes >= mediaDependentes)) {
        System.out.println("Funcionario deve receber auxilio.");
    }

    boolean salarioBaixo = salarioMensal < mediaSalario;
    boolean muitosDependentes = quantidadeDependentes >= mediaDependentes;

    if ((salarioBaixo) && (muitosDependentes)) {
        System.out.println("Funcionario deve receber auxilio.");
    }

    boolean recebeauxilio = (salarioBaixo) && (muitosDependentes);
    if (recebeauxilio = (salarioBaixo) && (muitosDependentes));
    if(recebeauxilio) {
    } else {
        System.out.println("Funcionario nao deve receber auxilio");
    }

    }

private  static  void  switchSemana() {

    String dia = "Terca";
    switch (dia) {
        case "Segunda":
            System.out.println(2);
            break;
        case "Terca":
            System.out.println(3);
            break;
        case "Qaurta":
            System.out.println(4);
            break;
        case "Quinta":
            System.out.println(5);
            break;
        case "Sexta":
            System.out.println(6);
            break;
        case "Sabado":
            System.out.println(7);
            break;
//        case "Domingo":
//            System.out.println(1);
//            break;
        default:
            System.out.println(1);
//            System.out.println("Dia invalido");
            break;
    }
    }

    private static void switchNumero() {

        int numero = 4 ;
        switch (numero){
            case 1:
            case 2:
            case 3:
                System.out.println("Certo");
                break;
            case 4:
                System.out.println("Errado");
                break;
            case 5:
                System.out.println("Talzez");
                break;
            default:
                System.out.println("Valor indefinido");
                break;
        }
    }

    private static  void switchFerias() {

        String mes = "dezembro";
        switch (mes) {
            case "dezembro":
            case"julho":
            case"janeiro":
                System.out.println("Ferias");
                break;
            default:
                System.out.println("Mes indefinido");
                break;
        }
    }
}
           //Resultado - primeira parte
Setembro
Setembro
Ferias
Funcionario nao deve receber auxilio
3
Errado
Ferias


###  //    Comentario  ,  código melhorado //

Erro de Codificação

na linha 22 se trocarmos o 9 por 20, 
que não esta presente na linha 57 Dezembro.
Na linha 149 "mxmx" qualquer texto  que mostra  vai voltar 1 dar valor Domingo
foi usado de forma erronea  o comprotamento padrao assumiu
valor de negocio e  transformou comportamento esperado o comportamento,
o comportamento padrao deve ser usado para dizer  algo inesperado aconteceu o valor que vc passou
não consegui trabalhar com ele.

// Resultado

Dezembro
Setembro
Ferias
Funcionario nao deve receber auxilio
3
Errado
Ferias


Melhorou o código substituindo
Linha 55 a 59 foi feito alteração


                                                    } else {
                                                    if (mes ==12) {
                                                    System.out.println("Dezembro");
                                                   } else {
                                                        System.out.println("Mes indefinido");


linha 168 a 173

        case "Domingo":
            System.out.println(1);
           break;
        default:
//            System.out.println(1);
            System.out.println("Dia invalido");
            
            
            ### Resultado final
            
 package dio.com.br;

/**
 * Classe de exemplo para o exercicio  da Aula 3 de Operadores lógicos e relacionais, controle de fluxo e Blocos.
 */
public class Main {

    public static void main(String[] args) {

        ifFlecha();
        ifSemFlecha();
        ifFerias();
        ifMenor();

        switchSemana();
        switchNumero();
        switchFerias();
    }

    private static void ifFlecha() {

        int mes = 20;
        if (mes == 1) {
            System.out.println("Janeiro");
        } else {
            if (mes == 2) {
                System.out.println("Fevereiro");
            } else {
                if (mes == 3) {
                    System.out.println("Março");
                } else {
                    if (mes == 4) {
                        System.out.println("Abril");
                    } else {
                        if (mes == 5) {
                            System.out.println("Maio");
                        } else {
                            if (mes == 6) {
                                System.out.println("Junho");
                            } else {
                                if (mes == 7) {
                                    System.out.println("Junho");
                                } else {
                                    if (mes == 8) {
                                        System.out.println("Agosto");
                                    } else {
                                        if (mes == 9) {
                                            System.out.println("Setembro");
                                        } else {
                                            if (mes == 10) {
                                                System.out.println("Outubro");
                                            } else {
                                                if (mes == 11) {
                                                    System.out.println("Novembro");
                                                } else {
                                                    if (mes ==12) {
                                                    System.out.println("Dezembro");
                                                   } else {
                                                        System.out.println("Mes indefinido");
                                               }
                                            }
                                        }
                                    }
                                }
                            }
                        }
                    }
                }
            }
        }
    }
}

    private static void ifSemFlecha () {

    int mes = 9;
    if (mes == 1) {
        System.out.println("Janeiro");
    } else if (mes == 2) {
        System.out.println("Fevereiro");
    } else if (mes == 3) {
        System.out.println("Março");
    } else if (mes ==4) {
        System.out.println("Abril");
    } else if (mes == 5) {
        System.out.println("Maio");
    } else if (mes == 6) {
        System.out.println("Junho");
    } else if (mes == 7) {
        System.out.println("Julho");
    } else if (mes == 8) {
        System.out.println("Agosto");
    } else if (mes == 9) {
        System.out.println("Setembro");
    } else if (mes == 10) {
        System.out.println("Outubro");
    } else if (mes == 11) {
        System.out.println("Novembro");
    } else {
        System.out.println("Dezembro");
    }
//    } else if (mes == 12)
//        System.out.println("Dezembro");
//    } else {
//        System.out.println("Mes indefinido");
//
//    }
}

    private static void ifFerias() {

        String mes = "julho";
        if (mes =="julho" || mes == "dezembro" || mes == "janeiro") {
            System.out.println("Ferias");
        }
    }

    private static void ifMenor() {

    double salarioMensal = 11893.58d;
    double mediaSalario = 10500d;

    int quantidadeDependentes = 4;
    int mediaDependentes = 2;

    if (salarioMensal < mediaSalario && (quantidadeDependentes >= mediaDependentes)) {
        System.out.println("Funcionario deve receber auxilio.");
    }

    boolean salarioBaixo = salarioMensal < mediaSalario;
    boolean muitosDependentes = quantidadeDependentes >= mediaDependentes;

    if ((salarioBaixo) && (muitosDependentes)) {
        System.out.println("Funcionario deve receber auxilio.");
    }

    boolean recebeauxilio = (salarioBaixo) && (muitosDependentes);
    if (recebeauxilio = (salarioBaixo) && (muitosDependentes));
    if(recebeauxilio) {
    } else {
        System.out.println("Funcionario nao deve receber auxilio");
    }

    }

private  static  void  switchSemana() {

    String dia = "mxmx";
    switch (dia) {
        case "Segunda":
            System.out.println(2);
            break;
        case "Terca":
            System.out.println(3);
            break;
        case "Quarta":
            System.out.println(4);
            break;
        case "Quinta":
            System.out.println(5);
            break;
        case "Sexta":
            System.out.println(6);
            break;
        case "Sabado":
            System.out.println(7);
            break;
        case "Domingo":
            System.out.println(1);
           break;
        default:
//            System.out.println(1);
            System.out.println("Dia invalido");
            break;
       }
    }

    private static void switchNumero() {

        int numero = 4 ;
        switch (numero){
            case 1:
            case 2:
            case 3:
                System.out.println("Certo");
                break;
            case 4:
                System.out.println("Errado");
                break;
            case 5:
                System.out.println("Talzez");
                break;
            default:
                System.out.println("Valor indefinido");
                break;
        }
    }

    private static  void switchFerias() {

        String mes = "dezembro";
        switch (mes) {
            case "dezembro":
            case"julho":
            case"janeiro":
                System.out.println("Ferias");
                break;
            default:
                System.out.println("Mes indefinido");
                break;
        }
    }
}



 ||| ## |||
 
Mes indefinido
Setembro
Ferias
Funcionario nao deve receber auxilio
Dia invalido
Errado
Ferias
