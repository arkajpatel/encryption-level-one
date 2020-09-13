# encryption-level-one
def enc(a):
	d = []
	q = []
	u = []
	for i in a:
		g = ord(i)
		d.append(g)
	o = str(sum(d))
	k = o[0]
	f = (int(k)//len(a))
	for i in d:
		f += i
		q.append(chr(f))
	
	return "".join(q)
a = input()
print(enc(a))
