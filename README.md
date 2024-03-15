import org.junit.Test;
import static org.junit.Assert.*;

public class CheckItTest {

    @Test
    public void testPredicateTrue() {
        assertTrue(CheckIt.checkIt(true, false, false));
    }

    @Test
    public void testPredicateFalse() {
      assertFalse(CheckIt.checkIt(false, false, false));
    }

    @Test
    public void testClauses() {
       
        assertTrue(CheckIt.checkIt(true, false, false)); 
        assertTrue(CheckIt.checkIt(false, true, true)); 
    }

    @Test
    public void testCACC() {
      
        assertTrue(CheckIt.checkIt(true, false, false));
        assertFalse(CheckIt.checkIt(false, false, false)); 
    }

    @Test
    public void testRACC() {
       
        assertTrue(CheckIt.checkIt(true, false, false)); 
        assertFalse(CheckIt.checkIt(false, true, false)); 
    }
}

![image](https://github.com/SOEN345-WINTER2024/logic-coverage-lab-jacksnj/assets/123913275/282687a0-de45-40da-b955-65941f5b0cf6)


