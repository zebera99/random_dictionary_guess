import random as rand
vocab = {}

with open('data/vocabulary.txt', 'r') as f:
    for line in f:
        data = line.strip().split(': ')
        eng, kor = data[0], data[1]
        vocab[eng] = kor

        keys = list(vocab.keys())
        index = rand.randint(0, len(keys) - 1)

        eng = keys[index]
        kor = vocab[eng]

        guess = input(f'{kor}: ')
        if guess == eng:
            print('맞았습니다!\n')
        elif guess == 'q':
            break
        else:
            print(f'틀렸습니다. 정답은 {eng}입니다.')
