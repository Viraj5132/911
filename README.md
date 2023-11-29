# 911
practical 2
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;
public class I {
   public static void main(String[] args) {
       // Set the path to the ChromeDriver executable
       System.setProperty("webdriver.chrome.driver", "C:/Users/kaust/Documents/Downloads/chromedriver-win64/chromedriver-win64/chromedriver.exe");
       // Create a new instance of the ChromeDriver
       WebDriver driver = new ChromeDriver();
       // Navigate to the Gmail login page
       driver.get("https://mail.google.com/");
       // Find the email input field and enter your email
       WebElement emailInput = driver.findElement(By.id("identifierId"));
       emailInput.sendKeys("k.sonkusare@gmail.com");
       // Click the "Next" button
       WebElement nextButton = driver.findElement(By.id("identifierNext"));
       nextButton.click();
       // Wait for a moment (you might need to add some explicit wait here)
       // Find the password input field and enter your password
       WebElement passwordInput = driver.findElement(By.name("password"));
       passwordInput.sendKeys("Kaustubh_1489");
       // Click the "Next" button
       WebElement passwordNextButton = driver.findElement(By.id("passwordNext"));
       passwordNextButton.click();
       // Wait for the Gmail dashboard to load (you might need to add some explicit wait here)
       // Close the browser
       driver.quit();
   }
}
