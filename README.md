# Building
import java.util.Scanner;

public class P04_Building {
    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        int countFloors = Integer.parseInt(scanner.nextLine());
        int countRooms = Integer.parseInt(scanner.nextLine());
        int currentfloor = countFloors;

        for (int basefloor = 0; basefloor < currentfloor ; currentfloor--) {

            for (int currentroom = 0; currentroom < countRooms ; currentroom++){

                if (countFloors == currentfloor) {
                    System.out.printf("L%d%d ", currentfloor, currentroom);
                }
                else if(currentfloor % 2 == 0){
                    System.out.printf("O%d%d ",currentfloor,currentroom);
                }
                else{
                    System.out.printf("A%d%d ",currentfloor,currentroom);
                }

            }
            System.out.println();
        }

    }

}
