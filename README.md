import java.util.Scanner;

public class Clock {

    public static double secondsToMinutes(int seconds) {
        return seconds / 60.0;
    }

    public static double secondsToHours(int seconds) {
        return seconds / 3600.0;
    }

    public static int minutesToSeconds(int minutes) {
        return minutes * 60;
    }

    public static double minutesToHours(int minutes) {
        return minutes / 60.0;
    }

    public static int hoursToSeconds(int hours) {
        return hours * 3600;
    }

    public static int hoursToMinutes(int hours) {
        return hours * 60;
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("Enter Seconds to convert into Minutes & Hours : ");
        int seconds = scanner.nextInt();
        System.out.println("Minutes : "+secondsToMinutes(seconds) );
        System.out.println("Hours : " + secondsToHours(seconds) );

        System.out.print("\nEnter Minutes to convert into Seconds & Hours : ");
        int minutes = scanner.nextInt();
        System.out.println("Seconds : " + minutesToSeconds(minutes) );
        System.out.println("Hours : " + minutesToHours(minutes) );

        System.out.print("\nEnter Hours to convert into Seconds & Minutes : ");
        int hours = scanner.nextInt();
        System.out.println("Seconds : " + hoursToSeconds(hours) );
        System.out.println("Minutes : " + hoursToMinutes(hours) );

        scanner.close();
    }
}
