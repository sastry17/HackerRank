#Decorators 2 - Name Directory

def person_lister(f):
    def inner(people):
        return [ f(i) for i in sorted(people, key = lambda x: (int(x[2])))]
    return inner