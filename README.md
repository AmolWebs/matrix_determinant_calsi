# matrix_determinant_calsi
# find determinant of any 2x2 or 3x3 matrix . 
# step 1 : install time library if you have'nt
# step 2 : Run the below code !!
import time
def display_board2(board):
    print('                  ')
    print('  ')
    print(board[1] + '|' + board[2])

    print(board[3] + '|' + board[4])
    print('    ')
    print('     ')

listed_board2 = ['m','a11','a12','a21','a22']



def display_board(board):
    print('                  ')
    print('  ')
    print(board[7] + '|' + board[8] + '|' + board[9])

    print(board[4] + '|' + board[5] + '|' + board[6])

    print(board[1] + '|' + board[2] + '|' + board[3])
    print('    ')
    print('     ')


listed_board = ['m', 'a31', 'a32', 'a31', 'a21', 'a22', 'a23', 'a11', 'a12', 'a13']



print('Welcome to the matrix calci , here you can find determinant of matrix ')
print('')
print('..............................................................')
selection = int(input('For 2x2 matrix press 2 \nor\nfor 3x3 matrix press 3 : '))

if selection == 2:
    print('Put your elements in downward format : ')
    display_board2(listed_board2)

    class Matrixes():
        def __init__(self, a, b, c, d):
            self.a = a
            self.b = b
            self.c = c
            self.d = d

        def determinant(self):
            q = self.a
            w = self.b
            e = self.c
            r = self.d
            print('your determinant value is ', (q * r) - (w * e))


    a = int(input('enter your a11 element '))
    b = int(input('enter your a21 element '))
    c = int(input('enter your a12 element '))
    d = int(input('enter your a22 element '))
    print('Processing...........')

    Mymatrix = Matrixes(a, b, c, d)
    Mymatrix.determinant()
    time.sleep(60)
elif selection == 3:
    print('Put your elements in downward format : ')
    display_board(listed_board)
    class Matrii():
        def __init__(self, a, b, c, d, e, f, g, h, i):
            self.a = a
            self.b = b
            self.c = c
            self.d = d
            self.e = e
            self.f = f
            self.g = g
            self.h = h
            self.i = i

        def determinant3(self):
            j = self.a
            k = self.b
            l = self.c
            m = self.d
            n = self.e
            o = self.f
            p = self.g
            q = self.h
            r = self.i
            print('  ')
            print('  ')
            print('Your determinant value is : ',
                  ((j * ((n * r) - (o * q))) - (m * ((k * r) - (l * q))) + (p * ((k * o) - (l * n)))))
            print('  ')


    a = int(input('Enter a11 element from matrix : '))
    b = int(input('Enter a21 element from matrix : '))
    c = int(input('Enter a31 element from matrix : '))
    d = int(input('Enter a12 element from matrix : '))
    e = int(input('Enter a22 element from matrix : '))
    f = int(input('Enter a32 element from matrix : '))
    g = int(input('Enter a13 element from matrix : '))
    h = int(input('Enter a23 element from matrix : '))
    i = int(input('Enter a33 element from matrix : '))
    threematri = Matrii(a, b, c, d, e, f, g, h, i)
    threematri.determinant3()
    print('...,.,.,,,,.,.,.,.,.,,,,,.,.,.,.,,.,,.,.,.,.,.,.,.,.,.,')
   
    print('restart for find another one value of determinanat')
    time.sleep(60)
  
 
