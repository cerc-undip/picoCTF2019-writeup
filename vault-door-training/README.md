# vault-door-training
**Category:** reverse <br>
**Point:** 50

> Your mission is to enter Dr. Evil's laboratory and retrieve the blueprints for his Doomsday Project. The laboratory is protected by a series of locked vault doors. Each door is controlled by a computer and requires a password to open. Unfortunately, our undercover agents have not been able to obtain the secret passwords for the vault doors, but one of our junior agents obtained the source code for each vault's computer! You will need to read the source code for each level to figure out what the password is for that vault door. As a warmup, we have created a replica vault in our training facility. The source code for the training vault is here: VaultDoorTraining.java

---

Deskripsi challenge ini cukup panjang, kita langsung menuju ke file-nya saja. Disini kita diberikan sebuah file `VaultDoorTraining.java`.

```java
import java.util.*;

class VaultDoorTraining {
  public static void main(String args[]) {
    VaultDoorTraining vaultDoor = new VaultDoorTraining();
    Scanner scanner = new Scanner(System.in); 
    System.out.print("Enter vault password: ");
    String userInput = scanner.next();
    String input = userInput.substring("picoCTF{".length(),userInput.length()-1);
    
    if (vaultDoor.checkPassword(input)) {
      System.out.println("Access granted.");
    } else {
      System.out.println("Access denied!");
    }
  }
  
  public boolean checkPassword(String password) {
      return password.equals("w4rm1ng_Up_w1tH_jAv4_fcb79c48f5b");
  }
}
```
Dapat dilihat bahwa program akan mengecek input dengan string `w4rm1ng_Up_w1tH_jAv4_fcb79c48f5b`, namun pengecekan string input dilakukan substring dengan `picoCTF{` sampai dengan `panjang input - 1`.

```zsh
➜  vault-door-training ✗ javac VaultDoorTraining.java
➜  vault-door-training ✗ java VaultDoorTraining 
Enter vault password: picoCTF{w4rm1ng_Up_w1tH_jAv4_fcb79c48f5b}
Access granted.
```

flag : `picoCTF{w4rm1ng_Up_w1tH_jAv4_fcb79c48f5b}`