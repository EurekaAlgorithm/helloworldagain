#project name and programming language
project('com.github.eurekaalgorithm.helloworldagain', 'vala', 'c')

#create a new executable, list the files I want to compile, list the dependencies 

executable(
	meson.project_name(),
	'src/Application.vala',
	dependencies: [
		dependency('gtk+-3.0')
	],
	install: true
)

#install my .desktop file so the Applications Menue will see it
install_data(
	join_paths('data',meson.project_name()+ '.desktop'),
	install_dir: join_paths(get_option('datadir'), 'applications')
)

#install the .appdata.xml file so AppCenter will see it
install_data(
	join_paths('data', meson.project_name() + '.appdata.xml'),
	install_dir: join_paths(get_option('datadir'), 'metainfo')
)
