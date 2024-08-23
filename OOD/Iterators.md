A way to iterate / go through any list or sequence
- Anything that can contains children
- Trees, Deque, Fibonacci, Cell

Iterator<T>{
	public boolean hasNext();
	public T next();
	public void remove()
}

To iterate, implement Iterator of sequence / object => pass in a specific sequence / object => use a while loop

## Iterable
After creating a class that implements Iteratable<T>, it can be used in a for-each loop

Iterable<T> {
	public Iterator<T> iterator();
}

To iterate, implement Iterator of sequence / object => define class as iterable => pass itself into iterator in iterator() => use a for-each loop