problem 1
float problemSolution1(float consumed_water) {
    float cost;
    // write your code here

    if (consumed_water <= 30.0) {
        cost = 13 + consumed_water * 0.4;
    } else if (consumed_water <= 50.0) {
        cost = 13 + 30.0 * 0.4 + (consumed_water - 30.0) * 0.12;
    } else if (consumed_water <= 60.0) {
        cost = 13 + 30.0 * 0.4 + 20.0 * 0.12 + (consumed_water - 50.0) * 1.4;
    } else {
        cost = 13 + 30.0 * 0.4 + 20.0 * 0.12 + 10.0 * 1.4 + (consumed_water - 60.0) * 1.5;
    }

    return cost;
}
problem 2
float problemSolution2(float i, float j, float k) {
    float result;
    // write your code here;
    i > j && i > k ? result = i : j > i && j > k ? result = j : result = k;

    return result;
}
problem 3 
#include <string>

std::string problemSolution3(float height, char S) {
    // write your code here
    std::string result;
    if (S == 'M') {
        if (height < 1.7) {
            result = "Short";
        } else if (height >= 1.7 && height < 1.85) {
            result = "Normal";
        } else if (height >= 1.85) {
            result = "Tall";
        }
    } else if (S == 'F') {
        if (height < 1.6) {
            result = "Short";
        } else if (height >= 1.6 && height < 1.75) {
            result = "Normal";
        } else if (height >= 1.75) {
            result = "Tall";
        }
    }

    // use return to return your result
    return result;
    // make use of control flow statements
}
problem 4
#include <string>
#include <sstream>

std::string problemSolution4(const std::string &macAddress) {
    // write your code here
    std::string result;
    if (macAddress[0] == 'F' and macAddress[1] == 'F') {
        result = "Broadcast";
    } else if ((int)macAddress[1] % 2 == 0) {
        result = "Unicast";
    } else if ((int)macAddress[1] % 2 == 1) {
        result = "Multicast";
    }
    
    return result;    
    // make use of control flow statements
    // return result;
}
problem 5
float problemSolution5(float x, float y, char operation) {
   float result;
   // write your code here
   if(operation=='+'){
      result=x+y;
   }else if(operation=='-'){
      result=x-y;
  }else if(operation=='*'){
      result=x*y;
   } else if(operation=='/'){
      result=x/y;
   }

   return result;
} 
