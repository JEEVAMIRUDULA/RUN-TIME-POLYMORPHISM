# RUN-TIME-POLYMORPHISM
package runtime.polymorphisim;

/**
 *
 * @author 1BSCCSA38
 */
class Grade{
    void belong(){
        System.out.println("Student belongs to:");
    }
}
class Primary extends Grade{
    @Override
    void belong(){
        System.out.println("Student belongs to primary grade");        
    }
}
class Secondary extends Grade {
    @Override
    void belong(){
        System.out.println("Student belongs to Secondary Grade");
    }
}
public class Runtime Polymorphism {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Grade grade;
        grade = new Primary();
        grade.belong();
        grade = new Secondary();
        grade.belong();
    }
    
}

o/p:

Student belongs to primary grade
Student belongs to Secondary Grade
