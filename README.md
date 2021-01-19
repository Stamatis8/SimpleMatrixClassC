# SimpleMatrixClassC++
As the name suggest, this is a simple matrix class in c++. It depends on the std::vector object. 
General:
Each matrix is saved in two ways, two std::vector<std::vector<double>> objects are attributes of the class, one named "Rows" and the other "Columns", where the rows and the columns are contained respectively.
Every operation on a matrix object that occurs automatically changes the respective value in both the "Rows" and the "Columns" objects.
Constructors:
 1)"matrix(std::vector<int> Size, int Type = 0 );" Here you pass the size of the matrix and the type you want. For example "matrix({2,3},0)" creates a zero matrix of size {2,3}
Type implemented so far;
    Types Implemented:
    0->0 matrix.
 2)"matrix(std::vector<std::vector<double>> Input_Vecs, bool IsRow = true);" Here you pass a bunch of same sized vectors as a first argument, and as a second argument you specify if these vectors are the rows of your matrix or the columns.
 3)"matrix()" a blank constructor.
Members:
  Getters and Setters:
  1)"matrix.GetValue(int i, int j);" It should be noted here that i,j start from 1 and not 0. As a general rule whenever the user has to input indexes for rows/columns the indexing starts from 1. This is done so that textbook formulas can be implemented seemlesly.
  2)"matrix.ChangeValue(int i, int j, double NewValue);" Changes the value at the ith row and jth columns to "NewValue". Again i,j start from 1
  Operations On Object:
  1)"matrix.add(overloaded)" If parameter is a a matrix then if the operation is allowed the two matrices are added together and saved at the original one. If parameter is a double, the all values of original matrix are increased by that amount.
  2)"matrix.multiply(double c)" Basic scalar multiplication on original matrix.
  3)"matrix.subtract(matrix B)" Subtracts matrix B
  Operations:
  1)"A+B" returns a matrix of that operation. Make sure that A and B are the same size
  2)"A-B" returns a matrix of that operation. Make sure that A and B are the same size
  3)"A*B" returns a matrix of multiplication of A*B.
  
  
