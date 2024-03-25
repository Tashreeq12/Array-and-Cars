
public class SumOfArrayElements {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        
        int[]array = {1,2,5,6,3,4};
        int sum = 0;
        
        for (int num : array){
        sum +=num;
        }
    System.out.println("Sum of all the elements in the array:" +sum);
            
    // Creating objects of Car and ElectricCar
    Car car = new Car("Toyota", "Yaris");
    ElectricCar myElectricCar = new ElectricCar("Telsa", "Model S", 120);
    
    // Displaying car details
    System.out.println("Toyota Yaris");
    System.out.println("Telsa Model S");
    
    }
    
}
