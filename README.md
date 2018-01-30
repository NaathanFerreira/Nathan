from random import choice
print('\033[1;34;m=-'*20)
print('ESCOLHA: Pedra, Papel ou Tesoura')
print('=-'*20)
j = input('\033[1;33;mFaça sua escolha: ').strip().title()
lista = ['Pedra', 'Papel', 'Tesoura']
m = choice(lista)
if j == 'Pedra' and m == 'Papel':
    print('\033[1;31;mVocê perdeu! O Computador escolheu Papel')
elif j == 'Pedra' and m == 'Tesoura':
    print('\033[1;32;mYeaah, você venceu! O Computador escolheu Tesoura')
elif j == 'Papel' and m == 'Pedra':
    print('\033[1;32;mYeaah, você venceu! O Computador escolheu Pedra')
elif j == 'Papel' and m == 'Tesoura':
    print('\033[1;31;mVocê perdeu! O Computador escolheu Tesoura')
elif j == 'Tesoura' and m == 'Pedra':
    print('\033[1;31;mVocê perdeu! O Computador escolheu Pedra')
elif j == 'Tesoura' and m == 'Papel':
    print('\033[1;32;mYeaah, você venceu! O Computador escolheu Papel')
else:
    print('\033[1;33;mEMPATE! Ambos escolheram {}'.format(j))
