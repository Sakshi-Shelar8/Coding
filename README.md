public class Main {
    public static int calculateTimeToTop(int height, int climbSpeed, int slideSpeed) {
        int time = 0;
        int distanceClimbed = 0;
        
        while (distanceClimbed < height) {
            time++;
            distanceClimbed += climbSpeed;
            
            if (distanceClimbed >= height) {
                break;
            }
            
            distanceClimbed -= slideSpeed;
        }
        
        return time;
    }

    public static void main(String[] args) {
        int wallHeight = 30;
        int climbSpeed = 3;
        int slideSpeed = 2;
        
        
        int hoursToTop = calculateTimeToTop(wallHeight, climbSpeed, slideSpeed);
        System.out.println(hoursToTop);
    }
}
//# Coding
Smowcode test
