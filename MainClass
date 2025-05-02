import java.io.IOException;
import java.nio.file.Files;
import java.nio.file.Path;
import java.util.ArrayList;

public class MainClass {

    // Ascii Daten abspeichern
    public class Zeichen{
        int ascii;   // ascii
        int counter; // n times vorkommen
    }

    public static ArrayList<String> lesen(String path){

        ArrayList<String> lines = null;
        Path p;

        try{
            p = Path.of(path);
        }catch(Exception e){
            e.getStackTrace();
            System.out.println("path unexcepted");
        }finally {
            p = Path.of("src/datei.txt");
        }

        try{
            lines = (ArrayList<String>) Files.readAllLines(p);
        }
        catch(IOException e){
            System.out.println( e.getMessage());
            System.exit(1);
        }
        return lines;
    }


    public static void printAscii(Object[] zeichen,int flag){


        // line feed
        //arrays.sort
        // falls 1 dann das Array hinsichtlich der
        // Mehrheitserscheinung der Buchstaben neu aufbauen
        if(flag == 1){

        }
        System.out.println("Ascii | # times | ");
        for (int i = 0; i < zeichen.length; i++) {
            System.out.printf("%5d" + " |" + "%3d%7s\n", i, zeichen[i], "|");
        }
    }


    public static void main(String[]args) throws IOException {

        //*********************************
        ArrayList<String> lines = lesen("");
        //*********************************
        //byteArray einlesen
        //zeilenenden speichern

        // iterieren und zahlen der einzelnen char's in jeder Zeile
       for( String s : lines){

           //ascii counter increment
           for(int i = 0; i < s.length(); i++) {
                ++ascii[s.charAt(i)];
           }
       }
       printAscii(ascii);

    }
}
