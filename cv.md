
# Elagina Kseniya
#### Student of RS school
***
### Contact information:  
Phone: +7 920 386 48-11\
E-mail: KseniaElagina2003@gmail.com\
Telegram: @tnanguper
***
### Brief Self-Introduction: 
I am a third-year student at a university in Yaroslavl.\
I am studying at the Faculty of Informatics and Computer Engineering\ 
and I want to gain experience as a front-end developer.\  
In this course I plan to master the basics of this profession.
***
### Skills and Proficiency: 
* JS Basic
* Python
* Flutter development
* C++
***
#### Code Examples:
```
class PasswordField extends StatefulWidget {
  final String text;
  const PasswordField({Key? key, required this.text}) : super(key: key);

  @override
  _PasswordFieldState createState() => _PasswordFieldState();
}

class _PasswordFieldState extends State<PasswordField> {
  final textFieldFocusNode = FocusNode();
  final emailController = TextEditingController();
  final passwordController = TextEditingController();

  final emailFocusNode = FocusNode();
  final passwordFocusNode = FocusNode();
  bool _obscured = true;


  @override
  Widget build(BuildContext context) {
    return Container(
      width: 343,
      height: 56,
      padding: const EdgeInsets.symmetric(horizontal: 20, vertical: 4),
      clipBehavior: Clip.antiAlias,
      decoration: ShapeDecoration(
        color: Color(0xFFEEEEEE),

        shape: RoundedRectangleBorder(
          borderRadius: BorderRadius.circular(12.50),
        ),
      ),

      child:
      new TextFormField(


        keyboardType: TextInputType.visiblePassword,
        obscureText: _obscured,
        focusNode: textFieldFocusNode,
        controller: passwordController,
        decoration: InputDecoration(

          floatingLabelBehavior: FloatingLabelBehavior.never,
          hintText: widget.text,
          hintStyle: TextStyle(
            color: Color(0xFF8D8D8D),
            fontSize: 16,
            fontFamily: 'Raleway',
            fontWeight: FontWeight.w500,
          ),
          border: InputBorder.none,
          suffixIconConstraints: BoxConstraints(maxHeight: 24, maxWidth: 24),

          suffixIcon: SizedBox(
              width: 24,
              height: 24,
              child: IconButton(
                padding: const EdgeInsets.symmetric(horizontal: 0, vertical: 0),


                onPressed: () {

                  setState(() {
                    _obscured = !_obscured;
                    if (textFieldFocusNode.hasPrimaryFocus) return;
                    textFieldFocusNode.canRequestFocus = false;
                  });
                },
                icon: _obscured
                ? SvgPicture.asset('assets/icons/Eye_open.svg')
                : SvgPicture.asset('assets/icons/Eye_closed.svg'),

                  iconSize: 24,
                  color: Color(0xFF8D8D8D),

                style: IconButton.styleFrom(
                  minimumSize: Size.zero,
                  padding: EdgeInsetsDirectional.all(0.0),
              ),

          ),
          ),
        ),

      ),
    );
  }
}
```
#### Work Experience:
Developing a project at the university using flutter:\
creating an application for tracking the expiration date of products.





