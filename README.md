do $$
declare
a int = 1;
b int = 1;

begin
	
	while a <= 12 loop
	raise notice 'Tabuada do %', a;
		b = 1;
		while b <= 10 loop
		raise notice '% X % = %', a, b, (a*b);
		b = b + 1;
		end loop;
		raise notice '|--------';
	a = a + 1;
	end loop;
	
end;
$$  language plpgsql;
