#include <stdio.h>
#include <stdlib.h>
#include <locale.h>
#include <string.h>
#include <ctype.h>
#include <stdbool.h>
#include <Windows.h>




void paises(){
    
    int pais;
    setlocale(LC_ALL, "portuguese");
    printf("\n\t4 paisse ir�o disputar os Jogos Olimpicos de Ver�o de 2024 em Paris na Fran�a.\n\n");
    printf("\t\t\t\t\t**********************************************\n");
    printf("\t\t\t\t\t ESCOLHA O PAIS E DO ATLETA QUE SERA CADASTRADO\n");
    printf("\t\t\t\t\t 1 - BRASIL \n"); 
    printf("\t\t\t\t\t 2 - ESTADOS UNIDOS \n");
    printf("\t\t\t\t\t 3 - RUSSIA \n");
    printf("\t\t\t\t\t 4 - CHINA \n");
    printf("\t\t\t\t\t**********************************************\n");
    scanf("%d", &pais);

    getchar();
    system("CLS");
    
    switch (pais) {

    case 1:
        Brasil();

        break;

    case 2:
        EUA();

        break;

    case 3:
        China();

        break;

    case 4:
        Russia();

        break;

    default:
            printf("\n\t\t\t\tESSE PAIS N�O ESTA NA LISTA!\n");
            exit(1);
        break;
    }
    system("CLS");
}
void Brasil()
{
    char nome[50];
    char idade [50];
    char sexo[50];
    char altura [50];
    char peso [50];
    char equipe[50];

    printf("\n\t\t\t\t\t*****************************************\n");
    printf("\t\t\t\t\t\t    CADASTRO DE ATLETA!\n");
    printf("\n\n");
    printf("\t\t\t\t\t      DIGITE OS DADOS DO ATLETA: \n");
    printf("\t\t\t\t\t*****************************************\n");
    printf("\n\n");

    printf("\nNOME: ");
    scanf("%s", &nome);;
          
    printf("\nIDADE: ");
    scanf("%s", &idade);
       
    printf("\nSEXO: ");
    scanf("%s", &sexo);

    printf("\nALTURA: ");
    scanf("%s", &altura);


    printf("\nPESO: ");
    scanf("%s", &peso);

    printf("\nEQUIPE: ");
    scanf("%s", &equipe);

        
    FILE *Olimpiadas;
    Olimpiadas = fopen("Olimpiadas.txt","a");
    fprintf(Olimpiadas, "\nDados do atleta:\n\nPa�s: Brasil\n");

    if(Olimpiadas == NULL)
    {
        printf("\nARQUIVO TXT N�O EXISTE\n");
        fflush(stdout);
    } else
    {
        if(nome == NULL || idade == NULL || sexo == NULL || altura == NULL || peso == NULL || equipe == NULL)
        {
            printf("EXISTEM CAMPOS EM BRANCO!");
            sleep(2);
            exit(1);
        }
        else
        {
            int atleta;
            
            atleta=fprintf(Olimpiadas, "Nome: %s\nSexo: %s\nSexo: %s\nAltura: %s\nPeso: %s\nEquipe: %s\n", nome, idade, sexo, altura, peso, equipe);
            if (atleta==EOF)
            {
                printf("\nN�O FOI POSSIVEL CADASTRAR O ATLETA!\n");
                sleep(2);
            }
            fclose(Olimpiadas);
            
            fputs("\n\t\t\t\t\tATLETA CADASTRADO COM SUCESSO!\n", stdout);
            fflush(stdout);
            sleep(2);
            system("CLS");
        }
        Modalidades();
    }    
}
void EUA()
{
    char nome[50];
    char idade [50];
    char sexo[50];
    char altura [50];
    char peso [50];
    char equipe [50];
 
    printf("\n\t\t\t\t\t*****************************************\n");
    printf("\t\t\t\t\t\t    CADASTRO DE ATLETA!\n");
    printf("\n\n");
    printf("\t\t\t\t\t      DIGITE OS DADOS DO ATLETA: \n");
    printf("\t\t\t\t\t*****************************************\n");
    printf("\n\n");

        
    printf("\nNOME: ");
    scanf("%s", &nome);;
          
    printf("\nIDADE: ");
    scanf("%s", &idade);
       
    printf("\nSEXO: ");
    scanf("%s", &sexo);

    printf("\nALTURA: ");
    scanf("%s", &altura);


    printf("\nPESO: ");
    scanf("%s", &peso);

    printf("\nEQUIPE: ");
    scanf("%s", &equipe);
        
    FILE *Olimpiadas;
    Olimpiadas = fopen("Olimpiadas.txt","a");
    fprintf(Olimpiadas, "\nDados do atleta:\n\nPa�s: EUA\n");

    if(Olimpiadas == NULL)
    {
        printf("\nARQUIVO TXT N�O EXISTE\n");
        fflush(stdout);
    } else
    {
        if(nome == NULL || idade == NULL || sexo == NULL || altura == NULL || peso == NULL || equipe == NULL)
        {
            printf("EXISTEM CAMPOS EM BRANCO!");
            sleep(2);
            exit(1);
        }
        else
        {
            int atleta;
            
            atleta=fprintf(Olimpiadas, "Nome: %s\nSexo: %s\nSexo: %s\nAltura: %s\nPeso: %s\nEquipe: %s\n", nome, idade, sexo, altura, peso, equipe);
            if (atleta==EOF)
            {
                printf("\nN�O FOI POSSIVEL CADASTRAR O ATLETA!\n");
                sleep(2);
            }
            fclose(Olimpiadas);
            
            fputs("\n\t\t\t\t\tATLETA CADASTRADO COM SUCESSO!\n", stdout);
            fflush(stdout);
            sleep(2);
            system("CLS");
        }
        Modalidades();
    }    
}
void China()
{
    char nome[50];
    char idade [50];
    char sexo[50];
    char altura [50];
    char peso [50];
    char equipe [50];

    printf("\n\t\t\t\t\t*****************************************\n");
    printf("\t\t\t\t\t\t    CADASTRO DE ATLETA!\n");
    printf("\n\n");
    printf("\t\t\t\t\t      DIGITE OS DADOS DO ATLETA: \n");
    printf("\t\t\t\t\t*****************************************\n");
    printf("\n\n");

        
    printf("\nNOME: ");
    scanf("%s", &nome);;
          
    printf("\nIDADE: ");
    scanf("%s", &idade);
       
    printf("\nSEXO: ");
    scanf("%s", &sexo);

    printf("\nALTURA: ");
    scanf("%s", &altura);

    printf("\nPESO: ");
    scanf("%s", &peso);

    printf("\nEQUIPE: ");
    scanf("%s", &equipe);
   
    FILE *Olimpiadas;
    Olimpiadas = fopen("Olimpiadas.txt","a");
    fprintf(Olimpiadas, "\nDados do atleta:\n\nPa�s: China\n");

    if(Olimpiadas == NULL)
    {
        printf("\nARQUIVO TXT N�O EXISTE\n");
        fflush(stdout);
    } else
    {
        if(nome == NULL || idade == NULL || sexo == NULL || altura == NULL || peso == NULL || equipe == NULL)
        {
            printf("EXISTEM CAMPOS EM BRANCO!");
            sleep(2);
            exit(1);
        }
        else
        {
            int atleta;
            
            atleta=fprintf(Olimpiadas, "Nome: %s\nSexo: %s\nSexo: %s\nAltura: %s\nPeso: %s\nEquipe: %s\n", nome, idade, sexo, altura, peso, equipe);
            if (atleta==EOF)
            {
                printf("\nN�O FOI POSSIVEL CADASTRAR O ATLETA!!\n");
                sleep(2);
            }
            fclose(Olimpiadas);
            
            fputs("\n\t\t\t\t\tATLETA CADASTRADO COM SUCESSO!\n", stdout);
            fflush(stdout);
            sleep(2);
            system("CLS");
        }
        Modalidades();
    }    
}
void Russia()
{
    char nome[50];
    char idade [50];
    char sexo[50];
    char altura [50];
    char peso [50];
    char equipe[50];

    printf("\n\t\t\t\t\t*****************************************\n");
    printf("\t\t\t\t\t\t    CADASTRO DE ATLETA!\n");
    printf("\n\n");
    printf("\t\t\t\t\t      DIGITE OS DADOS DO ATLETA: \n");
    printf("\t\t\t\t\t*****************************************\n");
    printf("\n\n");

        
    printf("\nNOME: ");
    scanf("%s", &nome);
          
    printf("\nIDADE: ");
    scanf("%s", &idade);
       
    printf("\nSEXO: ");
    scanf("%s", &sexo);

    printf("\nALTURA: ");
    scanf("%s", &altura);

    printf("\nPESO: ");
    scanf("%s", &peso);

    printf("\n EQUIPE: ");
    scanf("%s", &equipe);
        
    FILE *Olimpiadas;
    Olimpiadas = fopen("Olimpiadas.txt","a");
    fprintf(Olimpiadas, "\nDados do atleta:\n\nPais: Russia\n");

    if(Olimpiadas == NULL)
    {
        printf("\nARQUIVO TXT N�O EXISTE\n");
        fflush(stdout);
    } else
    {
        if(nome == NULL || idade == NULL || sexo == NULL || altura == NULL || peso == NULL || equipe == NULL)
        {
            printf("EXISTEM CAMPOS EM BRANCO!");
            sleep(2);
            exit(1);
        }
        else
        {
            int atleta;
            
            atleta=fprintf(Olimpiadas, "Nome: %s\nSexo: %s\nSexo: %s\nAltura: %s\nPeso: %s\nEquipe: %s\n ", nome, idade, sexo, altura, peso, equipe);
            if (atleta==EOF)
            {
                printf("\nN�O FOI POSSIVEL CADASTRAR O ATLETA!\n");
                sleep(2);
            }
            fclose(Olimpiadas);
            
            fputs("\n\t\t\t\t\tATLETA CADASTRADO COM SUCESSO!\n", stdout);
            fflush(stdout);
            sleep(2);
            system("CLS");
        }
        Modalidades();
    }    
}

void Modalidades(){
    int modalidade;
    setlocale(LC_ALL, "portuguese");
    printf("\n\t\t\t\t\t4 MODALIDES IR�O SER DISPUTADAS NOS JOGOS OLIMPICOS.\n\n");
    printf("\t\t\t\t\t**********************************************\n");
    printf("\t\t\t\t\t ESCOLHA A MODALIDA QUE SERA CADASTRADO\n");
    printf("\t\t\t\t\t 1 - NATA��O \n"); 
    printf("\t\t\t\t\t 2 - BOXE \n");
    printf("\t\t\t\t\t 3 - ATLETISMO \n");
    printf("\t\t\t\t\t 4 - LEVANTAMENTO DE PESO \n");
    printf("\t\t\t\t\t**********************************************\n");
    scanf("%d", &modalidade);

    getchar();
    system("CLS");

    switch (modalidade) {

    case 1:
        Natacao();

        break;

    case 2:
        Boxe();

        break;

    case 3:
        Atletismo();

        break;

    case 4:
        Levantamento();

        break;

    default:
            printf("\n\t\t\t\tESSA MODALIDADE N�O ESTA NA LISTA!\n");
            exit(1);
        break;
    }
    system("CLS");
}
void Natacao()
{
    int nata;
    FILE *Olimpiadas;
    Olimpiadas = fopen("Olimpiadas.txt","a");
    fprintf(Olimpiadas, "\nModalidade: Nata��o");
    fclose(Olimpiadas);
    printf("\n\t\t\t\tPRESSIONE 1 PARA ACESSAR A PROXIMA TELA.\n\n");
    scanf("%d", &nata);
    getchar();
    system("CLS");

    switch (nata){
    case 1:
        alojamento();

        break;

    default:
        printf("\n\t\t\t\tESSA MODALIDADE N�O ESTA NA LISTA!");
        exit(1);
    break;
    }
}

void Boxe()
{
    int box;
    FILE *Olimpiadas;
    Olimpiadas = fopen("Olimpiadas.txt","a");
    fprintf(Olimpiadas, "\nModalidade: Boxe");
    fclose(Olimpiadas);

    printf("\n\t\t\t\tPRESSIONE 1 PARA ACESSAR A PROXIMA TELA.\n\n");
    scanf("%d", &box);
    getchar();
    system("CLS");

    switch (box){
    case 1:
        alojamento();

        break;

    default:
        printf("\n\t\t\t\tESSA MODALIDADE N�O ESTA NA LISTA!\n");
        system("CLS");
        exit(1);
    break;
    }
}

void Atletismo()
{
    int atm;
    FILE *Olimpiadas;
    Olimpiadas = fopen("Olimpiadas.txt","a");
    fprintf(Olimpiadas, "\nModalidade: Boxe");
    fclose(Olimpiadas);

    printf("\n\t\t\t\tPRESSIONE 1 PARA ACESSAR A PROXIMA TELA.\n\n");
    scanf("%d", &atm);
    getchar();
    system("CLS");

    switch (atm){
    case 1:
        alojamento();

        break;

    default:
        printf("\n\t\t\t\tESSA MODALIDADE N�O ESTA NA LISTA!\n");
        system("CLS");
        exit(1);
    break;
    }
}
void Levantamento()
{
    int pesos;
    FILE *Olimpiadas;
    Olimpiadas = fopen("Olimpiadas.txt","a");
    fprintf(Olimpiadas, "\nModalidade: Boxe");
    fclose(Olimpiadas);

    printf("\n\t\t\t\tPRESSIONE 1 PARA ACESSAR A PROXIMA TELA.\n\n");
    scanf("%d", &pesos);
    getchar();
    system("CLS");

    switch (pesos){
    case 1:
        alojamento();

        break;

    default:
        printf("\n\t\t\t\tESSA MODALIDADE N�O ESTA NA LISTA!\n");
        system("CLS");
        exit(1);
    break;
    }
}

void alojamento()
{
    int vila;
    setlocale(LC_ALL, "portuguese");
    printf("\n\tA VILA OLIMPICA DE PARIS ESTA LOCAIZADA NO DESTRITO DE SEINT-SAINT-DENIS DA CIDADE.\n");
    printf("\tCOTEM 2 ALOJAMENTOS CAPAZES DE ACOMODAR TODAS AS DELEGA��ES!\n");

    printf("\t\t\t\t\t**********************************************\n");
    printf("\t\t\t\t\t ESCOLHA UM DOS ALOJAMENTOS PARA SUA DELEGA��ES\n");
    printf("\t\t\t\t\t 1 - ALOJAMENTO A \n"); 
    printf("\t\t\t\t\t 2 - ALOJAMENTO B \n");
    printf("\t\t\t\t\t**********************************************\n");
    scanf("%d", &vila);

    getchar();
    system("CLS");

    switch (vila){
        case 1:
            Aloj_A();

            break;
        case 2:
            Aloj_B();

            break;
        
        default:
        printf("\n\t\t\t\tESSA OP��O N�O EXISTE!\n");
        system("CLS");
        exit(1);
    break;
    }
}
void Aloj_A()
{
    int aa;
    FILE *Olimpiadas;
    Olimpiadas = fopen("Olimpiadas.txt","a");
    fprintf(Olimpiadas, "\nAlojamento: A");
    fclose(Olimpiadas);
    
    printf("\n\t\t\t\t\tALOJAMENTO A SELECIONADO!\n\n");
    printf("\n\t\t\t\tPRESSIONE 1 PARA ACESSAR A PROXIMA TELA.\n\n");
    scanf("%d", &aa);
    getchar();
    system("CLS");

    switch (aa){
    case 1:
        Locais();

        break;

    default:
        printf("\n\t\t\t\tESSA OP��O N�O EXISTE!\n");
        system("CLS");
        exit(1);
    break;
    }
}
void Aloj_B()
{ 
    int ab;
    FILE *Olimpiadas;
    Olimpiadas = fopen("Olimpiadas.txt","a");
    fprintf(Olimpiadas, "\nAlojamento: B");
    fclose(Olimpiadas); 

    printf("\n\t\t\t\t\tALOJAMENTO B SELECIONADO!\n\n");
    printf("\n\t\t\t\tPRESSIONE 1 PARA ACESSAR A PROXIMA TELA.\n\n");
    scanf("%d", &ab);
    getchar();
    system("CLS");

    switch (ab){
    case 1:
        Locais();

        break;

    default:
        printf("\n\t\t\t\tESSA OP��O N�O EXISTE!\n");
        system("CLS");
        exit(1);
    break;
    }  
}
void Locais()
{
    int local;
    setlocale(LC_ALL, "portuguese");
    printf("\n\t\t\t\t\t\tOS ESPORTES OLIMPICOS IR�O ACONTECER NOS RESPECTIVOS LOCAIS:\n\n");
    printf("\t\t\t\t\t*************************************************************************\n");
    printf("\t\t\t\t\t 1 - NATA��O - SAINT-DENIS! \n"); 
    printf("\t\t\t\t\t 2 - BOXE - STADE ROLAND GARROS! \n");
    printf("\t\t\t\t\t 3 - ATLETISMO - STADE DE FRANCE! \n");
    printf("\t\t\t\t\t 4 - LEVANTAMENTO DE PESO - CENTRO DE CONVEN��ES DA PORTA DE VERSAILLES \n");
    printf("\t\t\t\t\t*************************************************************************\n");
    printf("\n\t\t\t\t\t\tESCOLHA UMA OP��O DE ACORDO COM A MODALIDADE DO ATLETA!\n");
    scanf("%d", &local);
    
    getchar();
    system("CLS");

    switch (local){
        case 1:
            saint_denis();

            break;
        case 2:
            roland_garros();

            break;
        case 3:
            stade_de_france();

            break;
        case 4:
            versailles();

            break;
        
        default:
        printf("\n\t\t\t\tESSA OP��O N�O EXISTE\n");
        system("CLS");
        exit(1);
    break;
    }
}

void saint_denis()
{
    int sd;
    FILE *Olimpiadas;
    Olimpiadas = fopen("Olimpiadas.txt","a");
    fprintf(Olimpiadas, "\nLocal: Ssaint-Denis!");
    fclose(Olimpiadas);

    printf("\n\t\t\t\t\tO LOCAL FOI SELECIONADO!\n\n");
    printf("\n\t\t\t\tPRESSIONE 1 PARA ACESSAR A PROXIMA TELA.\n\n");
    scanf("%d", &sd);
    getchar();
    system("CLS");

    switch (sd){
    case 1:
        equipamentos();

        break;
    
    default:
        printf("\n\t\t\t\tESSA OP��O N�O EXISTE!\n");
        system("cls");
        exit(1);
    }


}
void roland_garros()
{
    int rg;
    FILE *Olimpiadas;
    Olimpiadas = fopen("Olimpiadas.txt","a");
    fprintf(Olimpiadas, "\nLocal: Roland Garros");
    fclose(Olimpiadas);

    printf("\n\t\t\t\t\tO LOCAL FOI SELECIONADO!\n\n");
    printf("\n\t\t\t\tPRESSIONE 1 PARA ACESSAR A PROXIMA TELA.\n\n");
    scanf("%d", &rg);
    getchar();
    system("CLS");

    switch (rg){
    case 1:
        equipamentos();

        break;
    
    default:
        printf("\n\t\t\t\tESSA OP��O N�O EXISTE!\n");
        system("cls");
        exit(1);
    }
}
void stade_de_france()
{
    int sf;
    FILE *Olimpiadas;
    Olimpiadas = fopen("Olimpiadas.txt","a");
    fprintf(Olimpiadas, "\nLocal: Stade de France");
    fclose(Olimpiadas);

    printf("\n\t\t\t\t\tO LOCAL FOI SELECIONADO!\n\n");
    printf("\n\t\t\t\tPRESSIONE 1 PARA ACESSAR A PROXIMA TELA.\n\n");
    scanf("%d", &sf);
    getchar();
    system("CLS");

    switch (sf){
    case 1:
        equipamentos();

        break;
    
    default:
        printf("\n\t\t\t\tESSA OP��O N�O EXISTE!\n");
        system("cls");
        exit(1);
    }
}
void versailles()
{
    int vs;
    FILE *Olimpiadas;
    Olimpiadas = fopen("Olimpiadas.txt","a");
    fprintf(Olimpiadas, "\nLocal: Versailles");
    fclose(Olimpiadas);

    printf("\n\t\t\t\t\tO LOCAL FOI SELECIONADO!\n\n");
    printf("\n\t\t\t\tPRESSIONE 1 PARA ACESSAR A PROXIMA TELA.\n\n");
    scanf("%d", &vs);
    getchar();
    system("CLS");

    switch (vs){
    case 1:
        equipamentos();

        break;
    default:
        printf("\n\t\t\t\tESSA OPC�O N�O EXISTE!\n");
        system("cls");
        exit(1);
    }
}

void equipamentos(){
    char equipamento[50];

    printf("\n\t\t\t\t\t*****************************************\n");
    printf("\n\t\t\t\t\t\t    CADASTRO DE EQUIPAMENTOS!\n");
    printf("\n\t\t\t\t\t*****************************************\n");
    printf("\n\n");

    printf("\n\t\t\t\tDIGITE O NOME DOS EQUIPAMENTOS QUE JULGAR NECESSARIO PARA O ATLETA TREINAR!\n");

    printf("\nEQUIPAMENTOS:");
    scanf("%s", &equipamento);
      
    FILE *Olimpiadas;
    Olimpiadas = fopen("Olimpiadas.txt","a");
    fprintf(Olimpiadas, "\nCadastro de equipamentos\n");

    if(Olimpiadas == NULL)
    {
        printf("\nARQUIVO TXT N�O EXISTE\n");
        fflush(stdout);
    } else
    {
        if(equipamento == NULL)
        {
            printf("\nEXISTEM CAMPOS EM BRANCO!\n");
            sleep(2);
            exit(1);
        }
        else
        {
            int eq;
            
            eq=fprintf(Olimpiadas, "Equipamentos: %s\n", equipamento);
            if (eq==EOF)
            {
                printf("\nN�O FOI POSSIVEL CADASTRAR EQUIPAMENTO!\n");
                sleep(2);
            }
            fclose(Olimpiadas);
            
            fputs("\n\t\t\t\t\tEQUIPAMENTO CADASTRADO COM SUCESSO!\n", stdout);
            fflush(stdout);
            sleep(2);
            system("CLS");
        }
        medico();
    }    
}
void medico() {
    char nome[50];
    char funcao[50];

    printf("\n\t\t\t\t\t*****************************************\n");
    printf("\n\t\t\t\t\t\t    CADASTRO DE MEDICO!\n");
    printf("\n\t\t\t\t\t*****************************************\n");
    printf("\n\n");

    printf("NOME: \n");
    scanf("%s", &nome);

    printf("FUN��O: \n");
    scanf("%s", &funcao);

    FILE *Olimpiadas;
    Olimpiadas = fopen("Olimpiadas.txt","a");
    fprintf(Olimpiadas, "\nCadastro de medico\n");

    if(Olimpiadas == NULL)
    {
        printf("\nARQUIVO TXT N�O EXISTE\n");
        fflush(stdout);
    } else
    {
        if(nome == NULL || funcao == NULL) 
        {
            printf("\nEXISTEM CAMPOS EM BRANCO!\n");
            sleep(2);
            exit(1);
        }
        else
        {
            int md;
            
            md=fprintf(Olimpiadas, "Nome: %s\nFun��o: %s\n", nome, funcao);
            if (md==EOF)
            {
                printf("\nN�O FOI POSSIVEL CADASTRAR O MEDICO!\n");
                sleep(2);
            }
            fclose(Olimpiadas);
            
            fputs("\n\t\t\t\t\tMEDICO CADASTRADO COM SUCESSO!\n", stdout);
            fflush(stdout);
            sleep(2);
            system("CLS");
        }
        funcionarios();
    }    
}

void funcionarios() {
    char nome[50];
    char idade[50];
    char cargo[50];
    char funcao[50];

    printf("\n\t\t\t\t\t*****************************************\n");
    printf("\n\t\t\t\t\t\t    CADASTRO DE FUNCIONARIO!\n");
    printf("\n\t\t\t\t\t*****************************************\n");
    printf("\n\n");

    printf("NOME: ");
    scanf("%s", &nome);

    printf("IDADE: ");
    scanf("%s", &idade);

    printf("CARGO: ");
    scanf("%s", &cargo);

    printf("FUN��O: ");
    scanf("%s", &funcao);

    FILE *Olimpiadas;
    Olimpiadas = fopen("Olimpiadas.txt","a");
    fprintf(Olimpiadas, "\nCadastro de funcionarios\n");

    if(Olimpiadas == NULL)
    {
        printf("\nARQUIVO TXT N�O EXISTE\n");
        fflush(stdout);
    } else
    {
        if(nome == NULL || idade == NULL || cargo == NULL || funcao == NULL)
        {
            printf("EXISTEM CAMPOS EM BRANCO!");
            sleep(2);
            exit(1);
        }
        else
        {
            int func;
            
            func=fprintf(Olimpiadas, "Nome: %s\nIdade %s\nCargo: %s\nFun��o: %s\n", nome, idade, cargo, funcao);
            if (func==EOF)
            {
                printf("\nN�O FOI POSSIVEL CADASTRAR O FUNCIONARIO!\n");
                sleep(2);
            }
            fclose(Olimpiadas);
            
            fputs("\n\t\t\t\t\tFUNCIONARIO CADASTRADO COM SUCESSO!\n", stdout);
            fflush(stdout);
            sleep(2);
            system("CLS");
        }
        voluntario();
    }    
}

void voluntario(){
    char nome[50];
    char idade[50];
    char cargo[50];
    char funcao[50];

    printf("\n\t\t\t\t\t*****************************************\n");
    printf("\n\t\t\t\t\t\t    CADASTRO DE VOLUNTARIOS!\n");
    printf("\n\t\t\t\t\t*****************************************\n");
    printf("\n\n");

    printf("NOME: \n");
    scanf("%s", &nome);

    printf("IDADE: \n");
    scanf("%s", &idade);

    printf("CARGO: \n");
    scanf("%s", &cargo);

    printf("FUN��O: \n");
    scanf("%s", &funcao);

    FILE *Olimpiadas;
    Olimpiadas = fopen("Olimpiadas.txt","a");
    fprintf(Olimpiadas, "\nCadastro de voluntarios\n");

    if(Olimpiadas == NULL)
    {
        printf("\nARQUIVO TXT N�O EXISTE\n");
        fflush(stdout);
    } else
    {
        if(nome == NULL || idade == NULL || cargo == NULL || funcao == NULL)
        {
            printf("EXISTEM CAMPOS EM BRANCO!");
            sleep(2);
            exit(1);
        }
        else
        {
            int fun;
            
            fun=fprintf(Olimpiadas, "Nome: %s\nIdade %s\nCargo: %s\nFun��o: %s\n", nome, idade, cargo, funcao);
            if (fun==EOF)
            {
                printf("\nN�O FOI POSSIVEL CADASTRAR O VOLUNTARIO!\n");
                sleep(2);
            }
            fclose(Olimpiadas);
            
            fputs("\n\t\t\t\t\tVOLUNTARIO CADASTRADO COM SUCESSO!\n", stdout);
            fflush(stdout);
            sleep(2);
            system("CLS");
        }
        ler();
    }  

}

void PrimeiraTela()
{
    setlocale(LC_ALL, "portuguese");
    printf("\n\t\t\t\t\t*****************************************\n");
    printf("\t\t\t\t\t\t    SEJA BEM VINDO!\n");
    printf("\t\t\t\t\t*****************************************\n");
    printf("\t\t\t\t\t     O PROGAMA INICIARA EM SEGUNDOS\n");
    printf("\t\t\t\t\t*****************************************\n");
    sleep(4);
    printf("\n\t\t\t\t\t\t\tINICIANDO...\n\n");
    sleep(2);
    system("CLS");
    
    void Privacidade();{
        setlocale(LC_ALL, "portuguese");

        printf("\n\t\t\t\t\t***********************************\n");
        printf("\t\t\t\t\t     POLITICA DE PRIVACIDADE\n");
        printf("\t\t\t\t\t***********************************\n");
        printf("\n\tSua privacidade � uma grande responsabilidade para n�s.\n"

            "\tAo se cadastar em nossa plataforma, voc� nos fornece todas as informa��es pessoais.\n"
            "\tColetamos todos os seus dados com a finalidade de aprimorar os servi�os oferecidos e \n"
            "\tmelhorar a experiencia dos usuarios.\n"

            "\tA plataforma se compromete em proteger todos os dados pessoais de acessos n�o autorizados.\n\n");
 
    }
    
    void Termos(); {

        int escolher; 
        setlocale(LC_ALL, "portuguese");
        printf("\t\t\t\t\t        ESCOLHA UMA OP��O:\n\n");

        printf("\t\t\t\t\t***************************************\n");
        printf("\t\t\t\t\t 1 - EU LI E ACEITO OS TERMOS\n");
        printf("\t\t\t\t\t***************************************\n");
        printf("\t\t\t\t\t 2 - EU LI E RECUSO OS TERMOS\n");
        printf("\t\t\t\t\t***************************************\n");
        scanf("%d", &escolher);

        getchar();
        system("CLS");
       
        switch (escolher) {

        case 1:
            tipo_de_login();

            break;

        case 2:
                printf("\n\t\t\t\tOBRIGADO POR USAR NOSSO SOFTWARE, O PROGAMA SERA FILNALIZADO EM 4 SECUNDOS\n");    
                sleep(1); 
                printf(".\n");
                sleep(1); 
                printf(".\n");
                sleep(1); 
                printf(".\n");
                sleep(1); 
                printf(".\n");
                system("CLS");  
                exit(1);         
            break;
        
        default:
            printf("\n\t\t\t\tESSA OP��O N�O EXISTE!");
            break;
        }

        getchar();

    }
}

void tipo_de_login()
 {
    int tipo;
    setlocale(LC_ALL, "portuguese");
	printf("\t\t\t\t\t     PRESSIONE 1 PARA CADASTRAR USUARIO!   \n ");

    printf("\n\t\t\t\t\t*****************************************\n");
	printf("\t\t\t\t\t 1 - CADASTRAR NOVO USARIO\n");
	printf("\n\t\t\t\t\t*****************************************\n");
	scanf("%d", &tipo);

    getchar();
	system("CLS");

    switch(tipo) {

     case 1:
	      cadastrar_login();
          	   
          break;
	
	default:
	        
            printf("\n\t\t\t\tESSA OP��O N�O EXISTE! O PROGAMA SERA ENCERRADO EM 3 SEGUNDOS");
            sleep(3);
            exit(1);
	    break;

	}	
    system("CLS");
}

void cadastrar_login()
{
    int * cadastro;
    char usuario [50];
    char senha [50];
    char password [50];
    FILE *Olimpiadas;

    if((Olimpiadas = fopen("Login.txt","a")) !=NULL)
    {
        system("CLS");
        printf("\n\t\t\t\t\t**************************************\n");
        printf("\t\t\t\t\t           CADASTRAR LOGIN!   \n ");
        printf("\n\t\t\t\t\t**************************************\n");

        printf("\n\tDIGITE O USUARIO: ");
        scanf("%s", &usuario);

        printf("\n\tDIGITE A SENHA: ");
        scanf("%s", &senha);

        printf("\n\tDIGITE NOVAMENTE A SENHA: ");
        fflush(stderr);
        scanf("%s", &password);

        if(strcmp(senha, password)== 0)
        {
            cadastro = fprintf(Olimpiadas, "Login: %s\nSenha: %s\n", usuario, senha);
            
            if(cadastro == EOF){
                printf("ERRO NO CADASTRO!\n");
            } else {
                fclose(Olimpiadas);

                printf("\n\t\t\t\t\tUSUARIO CADASTRADO COM SUCESSO!\n\n");
                fflush(stderr);
                sleep(2);
                system("CLS");

                paises();

            }
        }else
         {
            printf("\nSENHA ERRADA, TENTE MAIS TARDE!");
            sleep(2);
            fflush(stdout);
            system("CLS");
            exit(1);
        }  
    }
}
void ler(){
    FILE *Olimpiadas;
    char leitura; 
    Olimpiadas = fopen("Olimpiadas.txt","r");
    if (Olimpiadas == NULL)        
    {
        printf("Erro ao tentar abrir o arquivo!");
        exit(1);
    }
        printf("Lendo e exibindo os dados do arquivo \n\n");
    do
    {  
        leitura = fgetc(Olimpiadas);
        
        printf("%c" , leitura);        
    }while (leitura != EOF); 
    
            fclose(Olimpiadas);
    system("pause");
}

int main() {
    PrimeiraTela();
    return 0;
}
