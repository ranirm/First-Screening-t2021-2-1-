import java.util.*;

public class Problem4 
{
	public static void main(String[] args) 
  {
		System.out.println("Multiple of numbers 1 to 9");
		List<Integer> inputList=Arrays.asList(1,2,8,9,12,46,76,82,15,20,30);
		List<Integer> inputCheckList=Arrays.asList(1,2,3,4,5,6,7,8,9);
		Map<Integer,Integer> outputMap = new HashMap<>();
		for(Integer num: inputCheckList) 
    {
			int count = 0;
			for(Integer num1: inputList) 
      {
				if(num1%num == 0)
					count++;
			}
			outputMap.put(num, count);
		}
		System.out.println(outputMap);
	}

}
